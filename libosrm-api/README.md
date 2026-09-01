# libosrm C++ API reference — generated output

Everything in this directory is generated. Do not hand-edit it.

It is the rendered C++ API reference for `libosrm`, produced from the public headers of
`Project-OSRM/osrm-backend` at pinned commit
[`e9abd4e0268c692210c4f8e6dcd1d184ff2c8f72`](https://github.com/Project-OSRM/osrm-backend/tree/e9abd4e0268c692210c4f8e6dcd1d184ff2c8f72)
— the tip of `master` on 2026-08-05, four commits after the `v26.8.0` release.

## Regenerating

The generator lives in the backend repo under `tools/api-docs/`. From a fresh checkout:

```sh
git clone https://github.com/Project-OSRM/osrm-backend && cd osrm-backend
git checkout e9abd4e0268c692210c4f8e6dcd1d184ff2c8f72
python tools/api-docs/build.py --output /tmp/libosrm-api
```

It needs `doxygen` and `node` on `PATH`; the renderer is fetched with
`npx --yes sourcey@3.6.5`, pinned to an exact version. Copy the result over this directory
**minus `_og/`** — GitHub Pages runs Jekyll on this repository and Jekyll drops
leading-underscore paths, and those files are only social-preview images.

Every file in this directory except this README is byte-for-byte what that command produces.

## What is covered

The scope is exactly the set of types that `docs/libosrm.md` in the backend repo tells
embedders to go and read in the headers: `osrm::OSRM`, `EngineConfig`, `Status`, every
`*Parameters` type under `include/engine/api`, `util::Coordinate` / `FloatCoordinate`, the
`util::json` sum type and `storage::StorageConfig`. Each symbol page links back to the exact
file and line at the pinned commit.
