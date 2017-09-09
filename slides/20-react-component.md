### React component

```js
  import { Component } from 'react'
  import { createStore } from 'redux'
  import * as action from './actions'
  import counter from './reducers'

  const store = createStore(counter)

  class Counter extends Component {

    increment() {
      store.dispatch(action.increment())
    }

    render() {
      return (
        <div>
          <button onClick={this.increment}>
            Increment Counter
          </button>
        </div>
      )
    }
  }
```
