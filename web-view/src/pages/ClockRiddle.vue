<template>
  <div id="access">
    <div class="card overwrite">
      <Solution :hint="lukasHint" value="7288883"></Solution>
    </div>
  </div>
</template>

<script>
import Solution from '../components/Solution.vue';
export default {
  name: "Access",
  components: {Solution},
  data: function () {
    return {
      lukasHint: "Wir fangen bei der {{L-2}} an.",
      solution: ""
    };
  },
  methods: {
    checkValue() {
    }
  }
};
</script>

<style scoped>

.overwrite {
  background-image: url("../assets/images/riddle_3.png");
}
/deep/ .button  {
    color: rgba(3, 4, 3, 0.65);
}
.solution-wrapper {
  background-color: rgba(0, 0, 0, 0.65);
}

</style>