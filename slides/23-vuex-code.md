### Vuex structure

```js
  // types.js
  export const INCREMENT = 'INCREMENT';

  // actions.js
  import * as types from './types';

  export const increment = ({ commit }) => {
    commit(types.INCREMENT);
  }

  // reducers.js
  import * as types from './types';

  const state = {
    counter: 0,
  };

  export const mutations = {
    [types.INCREMENT](state){
      state.counter++;
    },
  };
```
