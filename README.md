# FormBlessed extension source downloads

This repository hosts versioned corresponding-source downloads for the FormBlessed Chrome extension. Download the named source ZIP from Releases; the automatically generated GitHub repository archive contains this download index only.

## Version 0.1.3

- [Complete browser-extension source ZIP](https://github.com/bane163/formblessed-extension-source/releases/download/v0.1.3/FormBlessed-0.1.3-source.zip)
- Source revision: `4118d644fdf8023544a47904d3d38eca01c5237e`
- SHA-256: `6a5df77800b35bbe05ccdbd88afd37624cfd24ea279f20bc69b4e299324455aa`

The ZIP contains editable extension code, public assets, the exact dependency lockfile, build scripts and license/provenance notices. It excludes account data, credentials, private runtime configuration and hosted backend source. Hosted services are external APIs and are not needed to compile the browser extension.

Use Node.js 24. Extract the ZIP, run `npm ci`, then run:

```sh
VITE_DOCUMENT_WORKER_URL=https://formblessed-api.lavenberry.com npm run build:release
```

The unpacked extension is emitted to `dist/`. Preserve the copyright and dependency notices in the archive, including `provenance/COPYCAT-LICENSE.txt` and the complete GPL text. Their existing terms apply to the corresponding code; third-party files retain their own notices and terms.

The source archive was rebuilt using the canonical installed locked dependencies and produced byte-identical output. See the attached source-rebuild verification record for the scope of that check.
