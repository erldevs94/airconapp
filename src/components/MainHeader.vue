<template>
  <div>
    <q-header class="q-pa-sm bg-blue-1" elevated>
      <q-toolbar>
        <q-toolbar-title
          ><router-link to="/" class="logoText">
            <img
              src="../assets/imgs/logo.png"
              id="logo"
              alt="Air conditioning services"
            />
            <span class="text-subtitle2 text-grey-9">
              Airconditioning Services</span
            >
          </router-link></q-toolbar-title
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
                <q-item-section>
                  <router-link
                    style="text-decoration: none"
                    class="text-bold text-blue-1"
                    :to="route.path"
                    >{{ route.label }}</router-link
                  ></q-item-section
                >
              </q-item>
            </q-list>
          </q-menu>
        </q-btn>
      </q-toolbar>
    </q-header>
    <q-footer class="bg-blue-grey-10" elevated>
      <div itemscope itemtype="https://schema.org/HVACBusiness">
        <meta itemprop="name" content="Clean Aire" />
        <div
          itemprop="address"
          itemscope
          itemtype="https://schema.org/PostalAddress"
        >
          <meta itemprop="streetAddress" content="Casili" />
          <meta itemprop="addressLocality" content="Consolacion, Cebu" />
          <meta itemprop="addressRegion" content="VII" />
          <meta itemprop="postalCode" content="6001" />
        </div>
        <meta content="09918625382" itemprop="telephone" />
        <meta content="louwellcabilan08@gmail.com" itemprop="email" />
        <meta itemprop="url" content="https://clean-aire.netlify.app/" />
        <meta itemprop="openingHours" content="Mo-Sa 8:00-6:00" />
      </div>
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
#logo {
  max-width: 15rem;
  width: 100%;
}

#main_header_stick {
  position: sticky;
  top: 0;
  z-index: 999;
}

.text-subtitle2 {
  position: absolute;
  left: 45px;
  bottom: 0;
}
</style>
