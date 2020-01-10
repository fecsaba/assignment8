<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <br>
        <button class="btn btn-primary"
          @click="selectedComponent='appBlue'">Load Blue Template</button>
        <button class="btn btn-success"
                @click="selectedComponent='appGreen'">Load Green Template</button>
        <button class="btn btn-danger"
                @click="selectedComponent='appRed'">Load Red Template</button>
        <hr>
        <component :is="selectedComponent">
          <p>Content</p>
        </component>
<!--        <app-blue></app-blue>-->
<!--        <app-green></app-green>-->
<!--        <app-red></app-red>-->
      </div>
    </div>
  </div>
</template>

<script>


import Blue from "@/components/Blue";
import Green from "@/components/Green";
import Red from "@/components/Red";

export default {
  name: 'app',
  components: {
    appBlue: Blue,
    appGreen: Green,
    appRed: Red
  },
  data: function () {
    return {selectedComponent: 'appRed'}
  }
}
</script>

<style>

</style>
