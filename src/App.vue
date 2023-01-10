<template>
    <div class="container">
        <div class="row">
          <div class="col-xs-12">
            <br>
            <button @click="selectedComponent='appBlue'" class="btn-sm btn btn-primary">Blue</button>
            <button @click="selectedComponent='appGreen'" class="btn-sm btn btn-primary">Green</button>
            <button @click="selectedComponent='appRed'" class="btn-sm btn btn-primary">Red</button>

            <component :is="selectedComponent">
                <h3>Sky</h3>
                <h3 slot="title"> Grass </h3>
                <h3 slot="flower"> Flower</h3>
            </component>
          </div>
        </div>
    </div>
</template>


<script>

import Blue from './components/Blue.vue'
import Green from './components/Green.vue'
import Red from './components/Red.vue'

export default {
    data : function() {
      return {
          selectedComponent : "appBlue"
      }
    },

    components: {
      'appBlue' : Blue,
      'appGreen' : Green,
      'appRed' : Red,
    }
}
</script>

