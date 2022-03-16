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
    <div class="glow q-md text-h6 text-weight-bold">
     <q-btn  label="Search" color="rgb(76, 129, 146), rgb(192, 216, 215)"  @click="search = true"/>
       <q-dialog v-model="search">
      <q-search
        transition-prev="slide-right"
        transition-next="slide-left"
        swipeable
        animated
        v-model="slide"
        control-color="primary"
        navigation-icon="radio_button_unchecked"
        navigation
        padding
        height="200px"
        class="bg-white shadow-1 rounded-borders"
      >

        <q-search-slide :name="1" class="row no-wrap flex-center">
          <div class="hey q-mt-md text-center" >Hospital name Ward Name L.G.A</div>
        </q-search-slide>
        <q-search-slide :name="2" class="row no-wrap flex-center">

          <div class="q-mt-md text-center">Hospital name Ward Name L.G.A
          </div>
        </q-search-slide>
        <q-search-slide :name="3" class="row no-wrap flex-center">
          <div class="q-mt-md text-center">Hospital name Ward Name L.G.A
          </div>
        </q-search-slide>
        <q-search-slide :name="4" class="row no-wrap flex-center">

          <div class="q-mt-md text-center">Hospital name Ward Name L.G.A
          </div>
        </q-search-slide>
      </q-search>
    </q-dialog>

          </div>



  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import { ref } from 'vue';
export default  {
  name: 'PageIndex',
   setup () {
    return {
      search: ref(true),

      slide: ref(1),
      lorem: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus, ratione eum minus fuga, quasi dicta facilis corporis magnam, suscipit at quo nostrum!',

      stars: ref(3),

      slideVol: ref(39),
      slideAlarm: ref(56),
      slideVibration: ref(63)
    }
  }

}

</script>

<style scoped>
  *{
    background-image: linear-gradient(to right, rgb(76, 129, 146), rgb(192, 216, 215));
  }
  .glow{
    position: absolute;
    bottom: 65%;
    left: 47%;
  }
  .tobi {
    padding-top: 30px;
  }
  .hey {
    display: block;
  }
</style>
