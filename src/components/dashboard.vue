<template>
  <div>
    <div>
      <searchCondition/>
    </div>
    <div>
      <chartResult/>
    </div>
  </div>
</template>

<script>
import searchCondition from "@/components/searchCondition";
import chartResult from "@/components/chartResult";

export default {
  name: "dashboard",
  components: {
    searchCondition,
    chartResult
  },
  data: function(){
    return {
      dashboard:'dash'
    }
  },
  methods: {
    searchHandler: function() {

    }
  }
}
</script>

<style scoped>

</style>