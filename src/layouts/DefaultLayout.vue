<template>
  <v-layout class="aira-layout">
    <v-app-bar color="primary" class="position-fixed">
      <template v-slot:prepend>
        <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      </template>
      <v-app-bar-title>
        <v-img :width="200" src="@/assets/fontlogo-white.webp"></v-img>
      </v-app-bar-title>
      <!--template v-slot:append>
        <v-btn icon="mdi-theme-light-dark" @click="toggleTheme"></v-btn>
      </template-->
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" :floating="true" elevation="2" class="position-fixed">
      <DrawerContent />
    </v-navigation-drawer>

    <v-main>
      <slot></slot>
      <WhitePantyhoseFooter />
    </v-main>
  </v-layout>
</template>

<script setup>
import DrawerContent from "@/components/DrawerContent.vue";
import WhitePantyhoseFooter from "@/components/WhitePantyhoseFooter.vue"
</script>

<script>
export default {
  data: () => ({
    drawer: undefined,
  }),
}
</script>

<style scoped lang="scss">
.position-fixed {
  position: fixed !important;
}
</style>
