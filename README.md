<img src='https://github.com/ljlm0402/vuex-state-storage-sync/raw/images/logo.jpg' border='0' alt='logo' />

[Vuex](https://vuex.vuejs.org/) State and Storage([local](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage), [session](https://developer.mozilla.org/en-US/docs/Web/API/Window/sessionStorage)) Synchronization module

<img src="https://img.shields.io/npm/v/vuex-state-storage-sync.svg" alt="NPM Version" /> <img src="https://img.shields.io/npm/l/vuex-state-storage-sync.svg" alt="Package License" /> <img src="https://img.shields.io/github/v/release/ljlm0402/vuex-state-storage-sync" alt="Release Version" /> <img src="https://img.shields.io/npm/dm/vuex-state-storage-sync.svg" alt="NPM Downloads" />

<br />

## πΉGuide

### Install

```js
$ npm install --save vuex-state-storage-sync
```

### Usage

```js
import Vue from 'vue';
import Vuex from 'vuex';
import syncStateStorage from 'vuex-state-storage-sync';

Vue.use(Vuex);

export default new Vuex.Store({
  state: {
    // ...
  },
  getters: {
    // ...
  },
  mutations: {
    // ...
  },
  actions: {
    // ...
  },
  modules: {
    // ...
  }
  plugins: [
    syncStateStorage({
      storage: window.localStorage || window.sessionStorage, // Storage Types
      key: '',  // Storage Key Name
      path: [''] // State data to be synchronized to storage
    })
  ]
});
```

## π¬ Recommended Commit Message

|  When |  Commit Message  |
|:--------|:-----------|
| Add function | feat: β‘οΈ Add function |
| Fix bug | fix: π Fix bug |
| Refactoring | refactor: π  Refactoring |
| Add package | package: π¦ Add package |
| Fix readme | docs: π Fix readme |
| Improvements style | style: π Improvements style |

## π³ License

[MIT](LICENSE)
