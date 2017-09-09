### Redux structure

```js
  // types.js
  export const INCREMENT = 'INCREMENT'

  // actions.js
  import * as types from './types'

  export const increment = () => ({ type: types.INCREMENT })

  // reducers.js
  import * as types from './types'

  export default (state = 0, action) => {
    switch (action.type) {
      case types.INCREMENT:
        return state + 1
      default:
        return state
    }
  }
```
