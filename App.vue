<template>
<div class="z" :style="{'background-image':'url(https://i1.wp.com/guitarandlace.com/wp-content/uploads/2021/01/4-1.png?ssl=1)'}">
    <h1 style="text-align: center; background-color: pink; font-family: monopasce;"><i>PROJECT CV</i></h1>
  <div id="app" class="container">
    <div class="row py-4" style="font-family: cursive">
      <agenda-input />
    </div><br>
    <div class="row py-4" style="font-family: fantasy">
      <agenda-show />
    </div>
  </div>
</div>
</template>

<script>
import AgendaInput from "./components/AgendaInput.vue";
import AgendaShow from "./components/AgendaShow.vue";

export default {
  name: "app",
  components: {
    AgendaInput,
    AgendaShow,
  },
};
</script>
