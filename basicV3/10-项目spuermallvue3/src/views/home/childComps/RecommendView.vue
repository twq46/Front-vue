<template>
  <div class="recommend">
    <div v-for="item in recommends" class="recommendItem">
      <a :href="item.link">
        <img :src="item.image" alt="">
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "RecommendView",
  props:{
    recommends:{
      type:Array,
      default(){
        return []
      }
    }
  }
}
</script>

<style scoped>
  .recommend{
    display: flex;
    text-align: center;
    font-size: 12px;
    padding: 10px 0 20px;
    border-bottom: 10px solid #eee;
  }
  .recommendItem{
    flex: 1;
  }
  .recommendItem a img{
    width: 70px;
    height: 70px;
    margin: 3px 0;
  }
</style>
