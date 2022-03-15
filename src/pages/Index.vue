<template>
  <q-page class="flex column">



    <div class="col text-white text-center">
      <div class="tobi q-pb-md text-h2 text-weight-light">
        Hospitals
      </div>
      <div class="q-pt-md text-h6 text-weight-light">
        Closest to me
      </div>
    </div>
        <q-btn to="/search" class="glow q-pb-md text-h6 text-weight-bold"
         color="rgb(76, 129, 146), rgb(192, 216, 215)" label="Search" />
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default  {
  name: 'PageIndex',

}
</script>

<style scoped>
  *{
    background-image: linear-gradient(to right, rgb(76, 129, 146), rgb(192, 216, 215));
  }
  .glow{
    position: absolute;
    bottom: 65%;
    left: 42%;
  }
  .tobi {
    padding-top: 30px;
  }
</style>
