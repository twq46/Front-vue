<template>
<div>
  <h2>{{$store.state.counter}}</h2>
  <h2>{{$store.getters.powerCounter}}</h2>
  <h2>{{$store.getters.more20stu}}</h2>
  <h2>{{$store.getters.moreAgestu(25)}}</h2>
</div>
</template>

<script>
export default {
name: "helloVuex",


}
</script>

<style scoped>

</style>
