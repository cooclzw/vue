<template>
  <div >
    <componentC></componentC>
    <ul>
      <li v-for="(item,index) in list" v-text="item.name + '-' + item.age + '-' +index"></li>
    </ul>
  </div>
</template>

<script>
import componentC from './components/a'
export default {
  components:{componentC},
  name: 'HelloWorld',
  data () {
    return {
      hello: 'world',
      list:[
        {
          name:"dzw",
          age:25
        },
        {
          name: "tao",
          age: 30
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
