### Vue component

```html
  <template>
    <div>
      <button @click="increment">Increment Counter</button>
    </div>
  </template>

  <script>
  import { mapActions } from 'vuex'

  export default {
    methods: mapActions({
      increment: 'counter/increment',
    }),
  };
  </script>
```
