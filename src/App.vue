<script>
export default {
  data() {
    return {
      msg: 'Counter',
      count: 0
    }
  },
  methods:{
    inc() {this.count = parseInt(String(this.count)) + 1;},
    dec() {this.count -= 1;}
  }
}
</script>

<template>
  <h1>{{ msg }}</h1>
  <input v-model="count"> 
  <h1>{{count}}</h1>
  <button @click="inc">+</button>
  <button @click="dec">-</button>
</template>

<style>

</style>