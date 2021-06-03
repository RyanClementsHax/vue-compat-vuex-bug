# vue-compat-vuex-bug

This repo takes a default vue 2.x app with vuex and follows the steps outlined in the [@vue/compat upgrade workflow instructions](https://www.npmjs.com/package/@vue/compat#upgrade-workflow). This repo shows that when started, the following will appear in the console:
```
vue.runtime.esm-bundler.js?1786:1404 Uncaught TypeError: Cannot read property 'state' of undefined
    at Proxy.mappedState (vuex.esm.js?2f62:945)
    at ComputedRefImpl.reactiveEffect [as effect] (vue.runtime.esm-bundler.js?1786:343)
    at ComputedRefImpl.get value [as value] (vue.runtime.esm-bundler.js?1786:1165)
    at Object.get [as counter] (vue.runtime.esm-bundler.js?1786:4515)
    at Object.get (vue.runtime.esm-bundler.js?1786:9487)
    at Proxy.eval (HelloWorld.vue?fdab:3)
    at renderComponentRoot (vue.runtime.esm-bundler.js?1786:2550)
    at componentEffect (vue.runtime.esm-bundler.js?1786:7280)
    at reactiveEffect (vue.runtime.esm-bundler.js?1786:343)
    at effect (vue.runtime.esm-bundler.js?1786:318)
```

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```