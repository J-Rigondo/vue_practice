<template>
  <div>
    차트결과
    <button @click="totalHandler">전체추이조회</button>
    <div v-if="show">
      <totalPage/>
    </div>
  </div>
</template>

<script>
import totalPage from "@/components/totalPage";

export default {
  name: "chartResult",
  components: {
    totalPage
  },
  data: function(){
    return {
      show: false

    }
  },
  created() {
    this.EventBus.$on('params', function (payload){
      console.log('초기조회받아라')
      console.log(payload);
    })
  },
  mounted() {

  },

  methods: {
    totalHandler: function() {
      this.show = !this.show;
    }
  },
}
</script>

<style scoped>

</style>