<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h1>{{ test }}</h1>
    <hr>
    <div class="devices">
      <div class="item">{{ status }}</div>
      <div class="item">{{ devName }}</div>
     yes <md-switch v-model="switchButton"> </md-switch>no
    </div>
  </div>
</template>

 
<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    test: String,
  },
  data: () => {
    return {
      status: false,
      devName: 'test',
      switchButton: false,
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scope>
h1 {
  text-align: left;
  color: lightgrey;
}
hr {
  border-width: 0.5em;
  border-style: solid;
  color: #42b983;
}
.devices {
  color: white;
  display: inline-block;
}
.devices > .item {
  display: inline-block;
  margin: 1em 2em;
}
</style>
