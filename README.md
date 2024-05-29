# vcmi-test-data

Data needed to run unit tests for the VCMI game engine. It may only be used for VCMI's continuous integration.

To run the unit tests, the following files from a Heroes 3 installation are required:

```
.
└── h3_assets
    └── Data
        ├── H3bitmap.lod
        ├── H3sprite.lod
        └── HiScore.dat
```

The directory h3_assets is compressed and encrypted (cf. https://askubuntu.com/a/1125254/838763):
```
7za a -tzip -p -mem=AES256 h3_assets.zip h3_assets
```

The archive can be extracted like this:
```
7za x h3_assets.zip -p$PASSWORD
```

See https://github.com/vcmi/vcmi/blob/develop/.github/workflows/github.yml for more details.
