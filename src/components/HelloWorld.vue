<template>
  <div >
    <ul>
      <li v-for="(item,index) in list" v-text="item.name + '-' + item.age + '-' +index"></li>
    </ul>
  </div>
</template>

<script>
export default {
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

