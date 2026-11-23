# Changelog

## [0.1.1](https://github.com/codeparticle/modly.web/compare/desktop-v0.1.0...desktop-v0.1.1) (2026-11-19)


### Features

* **auth:** Desktop deep-link PKCE sign-in (MD-1185) ([3b1a55f](https://github.com/codeparticle/modly.web/commit/3b1a55f49c2b00099f135c09e3430fd84cba7b97))
* **MD-1114:** Bake sidecar build into beforeDev/beforeBuild ([0da0aa6](https://github.com/codeparticle/modly.web/commit/0da0aa6a09ae7befa004c79afd823d0f9b7ac1e2))
* **MD-1114:** CI sidecar bundles + workflow_call reuse for release path ([face108](https://github.com/codeparticle/modly.web/commit/face108dfffab4521db4eaa3638a457b825f698f))
* **MD-1186:** Release-please + updater endpoint foundation ([de18855](https://github.com/codeparticle/modly.web/commit/de1885507d03e1319673a2563385307ab6a2913e))
* **MD-1189:** Releases.modly.one updater proxy route ([c25f5ae](https://github.com/codeparticle/modly.web/commit/c25f5ae9ae1857bc44c033bacb71f96093f3e3db))
* **MD-1191:** KMS Ed25519 signing scripts + minisign envelope wrapper ([d1d7d0f](https://github.com/codeparticle/modly.web/commit/d1d7d0f7b1902722215e197d2db7d93e2c25da62))


### Bug Fixes

* **api:** Allow tauri://localhost + https://tauri.localhost CORS origins ([6433299](https://github.com/codeparticle/modly.web/commit/643329900f5d6e2b309be5e16a057e67a70a1851))
* **desktop-auth:** Local api fallback + show loopback errors ([b0b77b5](https://github.com/codeparticle/modly.web/commit/b0b77b50cc8acf4ffcb4e9af9a0e48162a03a3a4))
* **desktop-auth:** Local api fallback + show loopback errors ([e2fead3](https://github.com/codeparticle/modly.web/commit/e2fead3318a54696d69b6530ad8c4c81cf17a779))
* **desktop:** Bake VITE_MODLY_API_URL into Rust at build time ([7bc308d](https://github.com/codeparticle/modly.web/commit/7bc308df3d1556200b596ccf76b429fc516d623f))
* **desktop:** Widen CSP connect-src to allow *.dev.modly.one + *.staging.modly.one ([c1fd061](https://github.com/codeparticle/modly.web/commit/c1fd061d0bcdf58db666a51f5451fc38b2dee7a9))
* **MD-1114:** Use uv for localproxy sidecar build ([67f8d81](https://github.com/codeparticle/modly.web/commit/67f8d815adc6833bb560a5d51f9a75005370ad3e))

## Changelog

All notable changes to Modly Desktop are documented here.

This changelog is maintained automatically by [release-please](https://github.com/googleapis/release-please) based on [Conventional Commits](https://www.conventionalcommits.org/).
