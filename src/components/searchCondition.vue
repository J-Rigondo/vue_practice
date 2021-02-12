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
    console.log('초기 조회 실행')
    this.searchHandler();
  },
  methods: {
    searchHandler: function() {
      console.log('설치실행행')
     this.EventBus.$emit('params','heelo')
    }
  }
}
</script>

<style scoped>

</style>