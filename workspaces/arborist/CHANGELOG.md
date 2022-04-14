# Changelog

## [6.0.0](https://github.com/anthonysidesap/cli/compare/arborist-v5.0.6...arborist-v6.0.0) (2022-04-14)


### ⚠ BREAKING CHANGES

* **arborist:** this drops support for the `log` property
* **arborist:** the log option is no longer passed to the updated deps

### Features

* **arborist:** add named updates validation ([#4307](https://github.com/anthonysidesap/cli/issues/4307)) ([fbe48a8](https://github.com/anthonysidesap/cli/commit/fbe48a84047e0c5de31bdaa84707f0f8fdcef71d))
* **arborist:** refactor arborist bin to use consistent timing/logging ([d438d61](https://github.com/anthonysidesap/cli/commit/d438d61d4f689966de8f964afe212d1319b8d460))


### Bug Fixes

* added arborist action and updated template-oss ([#4215](https://github.com/anthonysidesap/cli/issues/4215)) ([aa538df](https://github.com/anthonysidesap/cli/commit/aa538df4c19f46d2e24e2635d1214176c662fcea))
* **arborist:** _findMissingEdges missing dependency due to inconsistent path separators ([#4261](https://github.com/anthonysidesap/cli/issues/4261)) ([0e7511d](https://github.com/anthonysidesap/cli/commit/0e7511d144bdb6624e4c0fdfb31b4b42ed2954c9))
* **arborist:** check if a spec is a workspace before fetching a manifest, closes [#3637](https://github.com/anthonysidesap/cli/issues/3637) ([#4371](https://github.com/anthonysidesap/cli/issues/4371)) ([2ba09cc](https://github.com/anthonysidesap/cli/commit/2ba09cc0d7d56a064aa67bbb1881d381e6504888))
* **arborist:** convert all sorting to string-locale-compare ([#4465](https://github.com/anthonysidesap/cli/issues/4465)) ([1b4385f](https://github.com/anthonysidesap/cli/commit/1b4385f85e8f6dd5015080cdd3e02a8fa3749ffd))
* **arborist:** correctly load overrides on workspace edges, closes [#4205](https://github.com/anthonysidesap/cli/issues/4205) ([fabcf43](https://github.com/anthonysidesap/cli/commit/fabcf431a63ecf93b56ae5d9a05ad4e7ef280c2a))
* **arborist:** do not audit in offline mode ([#4410](https://github.com/anthonysidesap/cli/issues/4410)) ([54cda96](https://github.com/anthonysidesap/cli/commit/54cda9697b776fae807966097315c7b836623743))
* **arborist:** dont skip adding advisories to audit based on name/range ([aa4a4da](https://github.com/anthonysidesap/cli/commit/aa4a4da336a6ec1963394fdbd06acb173c842d26)), closes [#4681](https://github.com/anthonysidesap/cli/issues/4681)
* **arborist:** ensure indentation is preserved ([#4218](https://github.com/anthonysidesap/cli/issues/4218)) ([510f0ec](https://github.com/anthonysidesap/cli/commit/510f0ecbc9970ed8c8993107cc03cf27b7b996dc))
* **arborist:** fix superfluous arguments ([#4464](https://github.com/anthonysidesap/cli/issues/4464)) ([63b3557](https://github.com/anthonysidesap/cli/commit/63b35578bd759cb5f3edaaef1c1122ecd0b27f48))
* **arborist:** fix unescaped periods ([#4462](https://github.com/anthonysidesap/cli/issues/4462)) ([f4c5f0e](https://github.com/anthonysidesap/cli/commit/f4c5f0e52679b1aa42db833fc23dc07d96cc904e))
* **arborist:** handle link nodes in old lockfiles correctly ([6f9cb49](https://github.com/anthonysidesap/cli/commit/6f9cb490e7299976c43c6a118036c130671fe188))
* **arborist:** identify and repair invalid nodes in the virtual tree ([bd96ae4](https://github.com/anthonysidesap/cli/commit/bd96ae4071f9cc8a65e741f414db12e98537971d))
* **arborist:** load actual tree on named updates ([1f853f8](https://github.com/anthonysidesap/cli/commit/1f853f8bf7cecd1222703dde676a4b664526141d))
* **arborist:** make sure resolveParent exists before checking props ([18b8b94](https://github.com/anthonysidesap/cli/commit/18b8b94357d8f57301fbaa0f1e5dc2cf1128bf3e))
* **arborist:** prioritize valid workspace nodes ([#4230](https://github.com/anthonysidesap/cli/issues/4230)) ([c99c215](https://github.com/anthonysidesap/cli/commit/c99c2151a868672c017f64ff0ecb12149a2fb095)), closes [#3637](https://github.com/anthonysidesap/cli/issues/3637)
* **arborist:** save bundleDependencies to package.json when reifying ([e631faf](https://github.com/anthonysidesap/cli/commit/e631faf7b5f414c233d723ee11413264532b37de))
* **arborist:** save workspace version ([#4578](https://github.com/anthonysidesap/cli/issues/4578)) ([e9a2981](https://github.com/anthonysidesap/cli/commit/e9a2981f55f84ff521ef597883a4e732d08ce1c1))
* **arborist:** shrinkwrap throws when trying to read a folder without permissions ([#4258](https://github.com/anthonysidesap/cli/issues/4258)) ([8c3b143](https://github.com/anthonysidesap/cli/commit/8c3b143ca20d0da56c0ce2764e288a4c203b9f93))
* **arborist:** update save exact ([b51b29c](https://github.com/anthonysidesap/cli/commit/b51b29c563fa97aa4fbf38250d1f04e879a8d961))
* **arborist:** use full location as tracker key when inflating ([#4300](https://github.com/anthonysidesap/cli/issues/4300)) ([9bdd1ac](https://github.com/anthonysidesap/cli/commit/9bdd1ace86300a8ee562027bbc5cb57d62dc7ba8)), closes [#4273](https://github.com/anthonysidesap/cli/issues/4273) [#4298](https://github.com/anthonysidesap/cli/issues/4298)
* **arborist:** when reloading an edge, also refresh overrides ([4d676e3](https://github.com/anthonysidesap/cli/commit/4d676e31a68f081b8553eff4e79db1f29acf47e1))
* ignore integrity values for git dependencies ([#4468](https://github.com/anthonysidesap/cli/issues/4468)) ([c608512](https://github.com/anthonysidesap/cli/commit/c608512ed03ccf87dc989cec2849d14bf034513a))
* **logout:** require proper auth.js from npm-registry-fetch ([90c384c](https://github.com/anthonysidesap/cli/commit/90c384ccccac32c80c481a04c438cbcbea82539c))
* make sure we loadOverrides on the root node in loadVirtual() ([99d8845](https://github.com/anthonysidesap/cli/commit/99d88454248f950b82652b592fe2b4d019c1060b))
* npm update --save ([#4223](https://github.com/anthonysidesap/cli/issues/4223)) ([cfd59b8](https://github.com/anthonysidesap/cli/commit/cfd59b8c81078f842328b13a23a234150842cd58))
* only call npmlog progress methods if explicitly requested ([#4644](https://github.com/anthonysidesap/cli/issues/4644)) ([668ec7f](https://github.com/anthonysidesap/cli/commit/668ec7f33b7a76f5e86a59f7e5a6c0e068a242b1)), closes [#3314](https://github.com/anthonysidesap/cli/issues/3314)
* **rebuild:** don't run lifecycle scripts twice on linked deps ([#4529](https://github.com/anthonysidesap/cli/issues/4529)) ([fbdb431](https://github.com/anthonysidesap/cli/commit/fbdb43138ab8e682efb7668767465e7066d43b9f))
* replace deprecated String.prototype.substr() ([#4667](https://github.com/anthonysidesap/cli/issues/4667)) ([e3da5df](https://github.com/anthonysidesap/cli/commit/e3da5df4152fbe547f7871547165328e1bf06262))
* set proper workspace repo urls in package.json ([#4476](https://github.com/anthonysidesap/cli/issues/4476)) ([0cfc155](https://github.com/anthonysidesap/cli/commit/0cfc155db5f11ce23419e440111d99a63bf39754))
* update readme badges ([#4658](https://github.com/anthonysidesap/cli/issues/4658)) ([2829cb2](https://github.com/anthonysidesap/cli/commit/2829cb28a432b5ff7beeeb3bf3e7e2e174c1121d))


* **arborist:** remove log option ([eef16c1](https://github.com/anthonysidesap/cli/commit/eef16c18aacfbfed8bcfc72407d2a1b0c5ea00bc))


### Documentation

* standardize changelog heading ([#4510](https://github.com/anthonysidesap/cli/issues/4510)) ([91f03ee](https://github.com/anthonysidesap/cli/commit/91f03ee618bc635f9cfbded735fe98bbfa9d643f))


### Dependencies

* @npmcli/arborist@4.3.1 ([8732f39](https://github.com/anthonysidesap/cli/commit/8732f393ee547e2eada4317613599517c1d8ec0a))
* @npmcli/arborist@5.0.0 ([d58e444](https://github.com/anthonysidesap/cli/commit/d58e4442b0a16c84219d5f80ab88ef68ad209918))
* @npmcli/arborist@5.0.4 ([679e569](https://github.com/anthonysidesap/cli/commit/679e569d5778aef312b37c1ba3bda0171366c9fb))
* @npmcli/arborist@5.0.5 ([c70232c](https://github.com/anthonysidesap/cli/commit/c70232cc12fd9b3b024c2c759edd708af2367b8d))
* @npmcli/arborist@5.0.6 ([42dc0b0](https://github.com/anthonysidesap/cli/commit/42dc0b03d60dc27602dab26a2f8cbfc17bf4ab40))
* @npmcli/metavuln-calculator@3.0.1 ([fcc6acf](https://github.com/anthonysidesap/cli/commit/fcc6acfa808aa556748544edf4e9b73262f77608))
* @npmcli/move-file@2.0.0 ([e9b25cd](https://github.com/anthonysidesap/cli/commit/e9b25cd66bef17e807a84e7b10384f5f4d0064b7))
* @npmcli/node-gyp@2.0.0 ([0e87cac](https://github.com/anthonysidesap/cli/commit/0e87cac8b6f09692f6bd1bf086aadbe323d127b5))
* @npmcli/package-json@2.0.0 ([4a9a705](https://github.com/anthonysidesap/cli/commit/4a9a705de6992a3e9eefecc6c0cf8da45a527c7a))
* @npmcli/template-oss@3.2.1 ([aac01b8](https://github.com/anthonysidesap/cli/commit/aac01b89caf6336a2eb34d696296303cdadd5c08))
* @npmcli/template-oss@3.2.2 ([#4639](https://github.com/anthonysidesap/cli/issues/4639)) ([a59fd2c](https://github.com/anthonysidesap/cli/commit/a59fd2cb863245fce56f96c90ac854e62c5c4d6f))
* **arborist:** update to latest major versions of npm deps ([e5b4fa6](https://github.com/anthonysidesap/cli/commit/e5b4fa6251f0c6b16d84d46d62f5b98ad755385f))
* bin-links@3.0.0 write-file-atomic@4.0.0 ([#4254](https://github.com/anthonysidesap/cli/issues/4254)) ([2ef9f98](https://github.com/anthonysidesap/cli/commit/2ef9f9847c11fe8c0c0494558fe77c15ac4dbc80))
* cacache@16.0.0 ([e26548f](https://github.com/anthonysidesap/cli/commit/e26548fb12a3bb23fbe32a336f1305e083aa51c0))
* cacache@16.0.1 ([f95396a](https://github.com/anthonysidesap/cli/commit/f95396a033b75e2a3e9aa83f0b06c527641027a4))
* libnpmpublish@6.0.1 ([087fdc4](https://github.com/anthonysidesap/cli/commit/087fdc4cb4d6582b2b628087f866e8ca8bc00934))
* npm-install-checks@5.0.0 ([ad99360](https://github.com/anthonysidesap/cli/commit/ad9936063f20829eb9d5358d056593883f17a57b))
* npm-registry-fetch@12.0.1 ([1bfc507](https://github.com/anthonysidesap/cli/commit/1bfc507f2a5afa02f04d4dea2fc6d151d4fef3ac))
* pacote@13.0.5 ([340fa51](https://github.com/anthonysidesap/cli/commit/340fa51f423a518a96c8015a67d8f6144a2e8051))
* ssri@9.0.0 ([a2781a3](https://github.com/anthonysidesap/cli/commit/a2781a367d62328d7f870de878f1b63d66593f4f))
* treeverse@2.0.0 ([1a90b9e](https://github.com/anthonysidesap/cli/commit/1a90b9e9ebe98cce83591e11312aaf41c830f835))

### [5.0.6](https://github.com/npm/cli/compare/arborist-v5.0.5...arborist-v5.0.6) (2022-04-13)


### Bug Fixes

* **arborist:** dont skip adding advisories to audit based on name/range ([aa4a4da](https://github.com/npm/cli/commit/aa4a4da336a6ec1963394fdbd06acb173c842d26)), closes [#4681](https://github.com/npm/cli/issues/4681)
* **arborist:** when reloading an edge, also refresh overrides ([4d676e3](https://github.com/npm/cli/commit/4d676e31a68f081b8553eff4e79db1f29acf47e1))

### [5.0.5](https://github.com/npm/cli/compare/arborist-v5.0.4...arborist-v5.0.5) (2022-04-06)


### Bug Fixes

* replace deprecated String.prototype.substr() ([#4667](https://github.com/npm/cli/issues/4667)) ([e3da5df](https://github.com/npm/cli/commit/e3da5df4152fbe547f7871547165328e1bf06262))
* update readme badges ([#4658](https://github.com/npm/cli/issues/4658)) ([2829cb2](https://github.com/npm/cli/commit/2829cb28a432b5ff7beeeb3bf3e7e2e174c1121d))


### Dependencies

* @npmcli/arborist@5.0.4 ([679e569](https://github.com/npm/cli/commit/679e569d5778aef312b37c1ba3bda0171366c9fb))
* @npmcli/move-file@2.0.0 ([e9b25cd](https://github.com/npm/cli/commit/e9b25cd66bef17e807a84e7b10384f5f4d0064b7))
* @npmcli/node-gyp@2.0.0 ([0e87cac](https://github.com/npm/cli/commit/0e87cac8b6f09692f6bd1bf086aadbe323d127b5))
* @npmcli/package-json@2.0.0 ([4a9a705](https://github.com/npm/cli/commit/4a9a705de6992a3e9eefecc6c0cf8da45a527c7a))
* npm-install-checks@5.0.0 ([ad99360](https://github.com/npm/cli/commit/ad9936063f20829eb9d5358d056593883f17a57b))
* ssri@9.0.0 ([a2781a3](https://github.com/npm/cli/commit/a2781a367d62328d7f870de878f1b63d66593f4f))
* treeverse@2.0.0 ([1a90b9e](https://github.com/npm/cli/commit/1a90b9e9ebe98cce83591e11312aaf41c830f835))

### [5.0.4](https://github.com/npm/cli/compare/arborist-v5.0.3...arborist-v5.0.4) (2022-03-31)


### Bug Fixes

* **arborist:** handle link nodes in old lockfiles correctly ([6f9cb49](https://github.com/npm/cli/commit/6f9cb490e7299976c43c6a118036c130671fe188))
* **arborist:** identify and repair invalid nodes in the virtual tree ([bd96ae4](https://github.com/npm/cli/commit/bd96ae4071f9cc8a65e741f414db12e98537971d))
* **arborist:** make sure resolveParent exists before checking props ([18b8b94](https://github.com/npm/cli/commit/18b8b94357d8f57301fbaa0f1e5dc2cf1128bf3e))
* make sure we loadOverrides on the root node in loadVirtual() ([99d8845](https://github.com/npm/cli/commit/99d88454248f950b82652b592fe2b4d019c1060b))
* only call npmlog progress methods if explicitly requested ([#4644](https://github.com/npm/cli/issues/4644)) ([668ec7f](https://github.com/npm/cli/commit/668ec7f33b7a76f5e86a59f7e5a6c0e068a242b1)), closes [#3314](https://github.com/npm/cli/issues/3314)

### [5.0.3](https://www.github.com/npm/cli/compare/arborist-v5.0.2...arborist-v5.0.3) (2022-03-17)


### Bug Fixes

* **arborist:** _findMissingEdges missing dependency due to inconsistent path separators ([#4261](https://www.github.com/npm/cli/issues/4261)) ([0e7511d](https://www.github.com/npm/cli/commit/0e7511d144bdb6624e4c0fdfb31b4b42ed2954c9))
* **arborist:** save workspace version ([#4578](https://www.github.com/npm/cli/issues/4578)) ([e9a2981](https://www.github.com/npm/cli/commit/e9a2981f55f84ff521ef597883a4e732d08ce1c1))


### Dependencies

* @npmcli/metavuln-calculator@3.0.1 ([fcc6acf](https://www.github.com/npm/cli/commit/fcc6acfa808aa556748544edf4e9b73262f77608))
* cacache@16.0.0 ([e26548f](https://www.github.com/npm/cli/commit/e26548fb12a3bb23fbe32a336f1305e083aa51c0))
* pacote@13.0.5 ([340fa51](https://www.github.com/npm/cli/commit/340fa51f423a518a96c8015a67d8f6144a2e8051))

### [5.0.2](https://www.github.com/npm/cli/compare/arborist-v5.0.1...arborist-v5.0.2) (2022-03-10)


### Bug Fixes

* **rebuild:** don't run lifecycle scripts twice on linked deps ([#4529](https://www.github.com/npm/cli/issues/4529)) ([fbdb431](https://www.github.com/npm/cli/commit/fbdb43138ab8e682efb7668767465e7066d43b9f))


### Documentation

* standardize changelog heading ([#4510](https://www.github.com/npm/cli/issues/4510)) ([91f03ee](https://www.github.com/npm/cli/commit/91f03ee618bc635f9cfbded735fe98bbfa9d643f))

### [5.0.1](https://www.github.com/npm/cli/compare/arborist-v5.0.0...arborist-v5.0.1) (2022-03-08)


### Bug Fixes

* set proper workspace repo urls in package.json ([#4476](https://www.github.com/npm/cli/issues/4476)) ([0cfc155](https://www.github.com/npm/cli/commit/0cfc155db5f11ce23419e440111d99a63bf39754))

## 2.0.0

* BREAKING CHANGE: root node is now included in inventory
* All parent/target/fsParent/etc. references set in `root` setter, rather
  than the hodgepodge of setters that existed before.
* `treeCheck` function added, to enforce strict correctness guarantees when
  `ARBORIST_DEBUG=1` in the environment (on by default in Arborist tests).

## 1.0.0

* Release for npm v7 beta
* Fully functional

## 0.0.0

* Proof of concept
* Before this, it was [`read-package-tree`](http://npm.im/read-package-tree)
