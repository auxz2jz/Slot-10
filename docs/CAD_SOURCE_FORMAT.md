# CAD source storage and rebuild process

The detailed v2 CadQuery generator is currently stored as five text-safe chunks:

- `src/generator.b64.part00`
- `src/generator.b64.part01`
- `src/generator.b64.part02`
- `src/generator.b64.part03`
- `src/generator.b64.part04`

Concatenating the files in lexical order produces one base64 string. Decoding that string produces `generator.py.gz`. Expanding the gzip stream produces `generate_outdoor_gym_v2.py`.

The source was stored this way because the connected GitHub write interface is text-oriented. The representation is lossless; the committed chunks total **25,064 base64 characters**.

## Manual reconstruction

```bash
cat src/generator.b64.part* | base64 -d > generator.py.gz
gzip -dc generator.py.gz > generate_outdoor_gym_v2.py
python -m py_compile generate_outdoor_gym_v2.py
python generate_outdoor_gym_v2.py
```

The GitHub Actions workflow performs these same steps and uploads the generated detailed CAD package as an artifact.

## Future refactor

The generator should eventually be split into normal editable Python modules and data/config files. Until that refactor is completed and verified against the current generated package, the chunked v2 generator remains the reproducible baseline.
