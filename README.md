# VUEJS
Tips and tricks with Vue.js

## Routes

### Update route params data when route changed

```js
  export default{
    data () {
      return {
        id: this.$route.params.id
      }
    },
    watch: {
      '$route' (to, from) {
        this.id = to.params.id
      }
    }
  }
```
