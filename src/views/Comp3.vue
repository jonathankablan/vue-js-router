<template>
  <transition mode="out-in" appear>
  <div class="card">
    <div class="card-header text-light" style="background: purple;"> Component 3 </div>
    <div class="card-body m-5">
        <p class="card-text"> C'est un super composant </p>
    </div>
  </div>
  </transition>
</template>

<script>
export default {
  name: 'Component3',
  created() {
    console.log('route: ', this.$route);
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@keyframes fadein {
  from {
    opacity: 0;
    transform: translateX(-150px);
  }
  to {

  }
}

@keyframes fadeout {
  to {
    opacity: 0;
    transform: translateX(150px);
  }
}

.v-enter-active {
  animation: fadein 1s;
}

.v-leave-active {
  animation: fadeout 1s;
}
</style>
