<template>
  <q-page class="">
    <div class="row q-col-gutter-sm q-pr" >
      <!-- <q-btn color="indigo" label="Button" v-for="n in 7" :key="`xl-${n}`" /> -->
      <q-card
      class="my-card text-white row-5"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
      <q-card-section class="">
        <div class="text-h6">Hospital Name</div>
        <div class="text-subtitle2">L.G.A</div>
      </q-card-section>

      <q-card-section class="">
        {{ lorem }}
      </q-card-section>
    </q-card>

      <q-card
      class="my-card text-white row-5"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
      <q-card-section >
        <div class="text-h6">Hospital Name</div>
        <div class="text-subtitle2">L.G.A</div>
      </q-card-section>

      <q-card-section class="">
        {{ lorem }}
      </q-card-section>
    </q-card>

      <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
      <q-card-section class="col-5">
        <div class="text-h6">Hospital Name</div>
        <div class="text-subtitle2">L.G.A</div>
      </q-card-section>

      <q-card-section class="">
        {{ lorem }}
      </q-card-section>
    </q-card>

      <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
      <q-card-section class="col-5">
        <div class="text-h6">Hospital Name</div>
        <div class="text-subtitle2">L.G.A</div>
      </q-card-section>

      <q-card-section class="">
        {{ lorem }}
      </q-card-section>
    </q-card>
    </div>
    </q-page>

</template>

  <script>
export default {
  setup () {
    return {
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
}
</script>

<style  scoped>
.my-card{
   width: 100%;
  max-width: 250px;
  height: 20%;
}

</style>
