<template>
  <div>
    조건 검색창
    <button @click="searchHandler">조회</button>
  </div>
</template>

<script>
export default {
  name: "searchCondition",
  data: function(){
    return {

    }
  },
  created() {
    console.log('searchCondition created')
  },
  mounted() {
    console.log('searchCondition mounted')
    this.searchHandler();
  },
  methods: {
    searchHandler: function() {
      console.log('searchCondition emit')
     this.EventBus.$emit('params','heelo')
    }
  }
}
</script>

<style scoped>

</style>