<template>
  <h1>hello</h1>
<ul>
  <li v-for="item in items" :key="item.message">
    {{ item.message }}
  </li>
</ul>
</template>

<script>
export default {
  name: "HelloWorld",
   props: {
    msg: String
},
 data() {  
    return {
      items: [{ message: "ellyes" }, { message: "ellyes" }, { message: "noam" }, { message: "noam" }, { message: "noam" }, ],
    };
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
