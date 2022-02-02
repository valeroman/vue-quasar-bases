<template>
  <q-page class="flex column">
    <!-- <h1>Typography</h1> -->
    <span class="text-h1">Headline 1</span>
    <span class="text-h2">Headline 2</span>
    <span class="text-h3">Headline 3</span>
    <span class="text-h4">Headline 4</span>
    <span class="text-h5">Headline 5</span>
    <span class="text-h6">Headline 6</span>

    <q-separator color="orange" />

    <span class="text-subtitle1">Subtitle1</span>
    <span class="text-subtitle2">Subtitle2</span>

    <q-separator color="orange" />

    <p class="text-body1">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias porro
      minima veniam? Alias molestias illo, quidem minus consectetur atque
      eligendi natus, impedit possimus aut dicta magni. Quae dolorem ducimus
      aperiam!
    </p>
    <p class="text-body2">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi
      reiciendis eaque praesentium ipsum aspernatur aliquam. Quaerat culpa ipsa
      quidem impedit, aliquam mollitia recusandae cum dolor commodi nesciunt
      sint labore itaque!
    </p>

    <q-separator color="orange" />

    <span class="text-weight-thin"
      >reiciendis eaque praesentium ipsum aspernatur aliquam. Quaerat culpa
      ipsa</span
    >
    <span class="text-weight-light"
      >reiciendis eaque praesentium ipsum aspernatur aliquam. Quaerat culpa
      ipsa</span
    >
    <span class="text-weight-regular"
      >quidem impedit, aliquam mollitia recusandae cum dolor commodi
      nesciunt</span
    >
    <span class="text-weight-medium"
      >Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias
      porro</span
    >
    <span class="text-weight-bold"
      >quidem impedit, aliquam mollitia recusandae cum dolor commodi
      nesciunt</span
    >
    <span class="text-weight-bolder"
      >Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias
      porro</span
    >

    <q-btn
      @click="toggleSideMenu"
      class="q-mt-md"
      color="primary"
      :label="sideMenuOpen ? 'Cerrar menu lateral' : 'Abrir menu lateral'"
    />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import useUI from "../composables/useUI";

export default defineComponent({
  name: "Typography",

  setup() {
    const { sideMenuOpen, toggleSideMenu } = useUI();

    return {
      toggleSideMenu,
      sideMenuOpen,
    };
  },
});
</script>
