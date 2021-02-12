<template>
  <div>
    totalpage
  </div>
</template>

<script>
export default {
  name: "totalPage",
  created() {
    //console.log(this.$parent.parentData)
    //console.log(this.$parent.$parent.dashboard)

    console.log('totalPage created')
    this.EventBus.$on('params', function (payload){
      console.log('totalPage on')
      console.log(payload);
    });
  },
  mounted() {
    console.log('totalPage mounted')
  }
}

</script>

<style scoped>

</style>