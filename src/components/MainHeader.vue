<template>
  <div>
    <q-header class="q-pa-sm bg-blue-1" elevated>
      <q-toolbar>
        <q-toolbar-title
          ><router-link to="/" class="logoText">
            <span class="q-pa-sm text-primary text-bold text-no-wrap logoText"
              >Clean Aire
              <span class="material-icons text-h4" glossy> ac_unit </span></span
            ></router-link
          ></q-toolbar-title
        >

            
        <q-btn flat icon="menu" label="Menu" class="text-primary">
          <q-menu
            style="width: 10rem"
            class="text-center"
            transition-show="flip-right"
            transition-hide="flip-left"
          >
            <q-list class="bg-primary">
              <q-item v-for="(route, index) in routes" :key="index">
                <q-item-section >
                  <router-link style="text-decoration: none;" class="text-bold text-blue-1" :to="route.path">{{
                    route.label
                  }}</router-link></q-item-section
                >
              </q-item>
            </q-list>
          </q-menu>
        </q-btn>
      </q-toolbar>
    </q-header>
    <q-footer class="bg-blue-grey-10" elevated>
      <q-toolbar>
        <q-toolbar-title>Clean Aire</q-toolbar-title>
        <small>Copyright <q-icon name="copyright"></q-icon> 2022</small>
      </q-toolbar>
    </q-footer>
  </div>
</template>

<script setup>
import { ref } from "vue";
const routes = ref([
  { label: "HOME", path: "/" },
  { label: "ABOUT", path: "/about" },
]);
</script>

<style scoped>
.logoText {
  text-decoration: none;
}

#main_header_stick {
  position: sticky;
  top: 0;
  z-index: 999;
}
</style>
