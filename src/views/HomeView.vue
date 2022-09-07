<template>
  <q-page>
    <div class="row">
      <div class="col-12 col-md-9">
        <q-carousel
          arrows
          swipeable
          animated
          v-model="slide"
          height="700px"
          infinite
          :autoplay="autoplay"
          @mouseenter="autoplay = false"
          @mouseleave="autoplay = true"
        >
          <q-carousel-slide
            name="first"
            img-src="../assets/imgs/checking-conditioner-min.jpg"
          >
            <q-btn href="#contact" class="bg-primary text-bold text-grey-2 float-right"
              >Request a quote</q-btn
            >
            <div class="absolute-bottom custom-caption">
              <div class="text-h2 text-primary">
                <span class="bg-blue-1 q-pa-sm rounded-borders"
                  >CLEAN AIRE</span
                >
              </div>
              <div class="text-subtitle1">
                <span class="bg-blue-1 q-pb-md q-px-md">Keeping You Cool</span>
              </div>
            </div>
          </q-carousel-slide>
          <q-carousel-slide name="second" img-src="../assets/imgs/aircon4.jpg">
            <q-btn href="#contact" class="bg-primary text-bold text-grey-2 float-right"
              >Request a quote</q-btn
            >
            <div class="absolute-bottom custom-caption">
              <div class="text-h2 text-primary">
                <span class="bg-blue-1 q-px-sm q-pb-sm rounded-borders"
                  >Aircon Services</span
                >
              </div>
              <!-- <div class="text-subtitle1">
                <span class="bg-blue-1 q-pb-md q-pa-md"
                  >Don’t sweat it, call
                  <span class="text-bold q-pb-md q-px-md">CLEAN AIRE</span>
                </span>
              </div> -->
            </div>
          </q-carousel-slide>
          <q-carousel-slide name="third" img-src="../assets/imgs/aircon8.jpg">
            <q-btn href="#contact" class="bg-primary text-bold text-grey-2 float-right"
              >Request a quote</q-btn
            >
            <div class="absolute-bottom custom-caption">
              <div class="text-h2 text-primary">
                <span class="bg-blue-1 q-pb-sm q-px-sm rounded-borders">
                  Home Service
                </span>
              </div>
              <!-- <div class="text-subtitle1">
                <span class="bg-blue-1 q-pb-md q-px-md"> We make cozy happen </span>
              </div> -->
            </div>
          </q-carousel-slide>
        </q-carousel>
      </div>
      <div class="col-12 col-md-3 q-pa-md row flex-center bg-blue-1">
        <div flat bordered class="about-card window-width">
          <q-card-section>
            <div class="text-h4 text-primary text-center">
              About Us
              <q-icon class="text-center" name="handyman" size="2rem"></q-icon>
            </div>
          </q-card-section>
          <q-card-section class="q-pa-xl">
            <p>
              We do cleaning both interior and exterior parts of the unit by
              using our reliable tools within our skills and experience for
              <span class="text-bold">6 years</span>.
            </p>
            <p>
              We also do inspection, repair and even overhaul of aircon units.
            </p>
            <p>
              Regular aircon servicing ensures better temperature control and
              cleaner air from a clean unit.
            </p>
            <p>
              Clients I've worked on:
              <span class="text-bold">
                Sendai Motors, Ascentia, Myvan properties</span
              >
            </p>
          </q-card-section>

          <!-- <q-separator inset />
          <q-card-section>
            <div class="text-h6"><q-icon name="call"></q-icon> Phone</div>
            <p>09918625382</p>
          </q-card-section>
          <q-card-section>
            <div class="text-h6">
              <q-icon name="perm_identity"></q-icon> Facebook
            </div>
            <p>
              <a
                href="https://www.facebook.com/profile.php?id=100009552072438"
                target="blank"
                >Louwell Cabilan</a
              >
            </p>
          </q-card-section> -->
        </div>
      </div>
    </div>
    <div class="col-12">
      <h4 class="text-center text-primary">
        Services Offered <q-icon name="home_repair_service"></q-icon>
      </h4>
      <div class="row q-col-gutter-xl q-pa-md">
        <div class="col-12 col-md-4">
          <q-card class="service-card q-mx-auto">
            <q-img src="../assets/imgs/service-1.jpg">
              <div class="absolute-bottom text-h6">Aircon Cleaning</div>
            </q-img>
            <q-card-section>
              <ul>
                <li>Wall mounted/Split Type</li>
                <li>Window Type</li>
              </ul>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-12 col-md-4">
          <q-card class="service-card q-mx-auto">
            <q-img src="../assets/imgs/service-2.jpg">
              <div class="absolute-bottom text-h6">Aircon Repair</div>
            </q-img>
            <q-card-section>
              <ul>
                <li>Wall Mounted/Split Type</li>
                <li>Window Type</li>
                <li>Ceiling Cassette</li>
                <li>Floor Standing</li>
                <li>Ceiling Suspended</li>
                <li>Etc.</li>
              </ul>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-12 col-md-4">
          <q-card class="service-card q-mx-auto">
            <q-img src="../assets/imgs/service-3.jpg">
              <div class="absolute-bottom text-h6">Aircon Installation</div>
            </q-img>
            <q-card-section>
              <ul>
                <li>Wall Mounted/Split Type</li>
                <li>Window Type</li>
                <li>Ceiling Cassette</li>
                <li>Floor Standing</li>
                <li>Ceiling Suspended</li>
              </ul>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
    <div class="row q-px-lg q-mt-lg" id="contact">
      <div class="col-12 col-md-8 bg-grey-2">
        <h1 class="text-bold">Chill out!</h1>
        <h6>Are you ready for the big chill?</h6>
      </div>
      <div class="col-12 col-md-4 bg-primary">
        <h1 class="text-grey-3 text-bold text-center">Let's Talk</h1>
        <h6 class="text-center text-white">
          <q-icon name="call"></q-icon>: 09918625382 /
          <q-icon name="mail"></q-icon>l.cabilan@yahoo.com / 
          <a
          class="text-bold text-white"
          href="https://www.facebook.com/profile.php?id=100009552072438"
          target="_blank"
        >Facebook</a>
        </h6>
       
      </div>
    </div>
  </q-page>
</template>

<script setup>
import { ref } from "vue";

const slide = ref("first");
const autoplay = ref(true);
</script>

<style scoped>
.service-card {
  width: 100%;
  max-width: 25rem;
}

.contact-us {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' version='1.1' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:svgjs='http://svgjs.com/svgjs' width='1440' height='560' preserveAspectRatio='none' viewBox='0 0 1440 560'%3e%3cg mask='url(%26quot%3b%23SvgjsMask1010%26quot%3b)' fill='none'%3e%3cpath d='M1218.1562945434603 284.9626616034936L1071.4969260297803 287.5226104032312 1220.716243343198 431.6220301171736z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M425.07393190121354-40.496661576300944L340.08619378674473-11.23303655245877 369.3498188105869 73.75470156201004 454.3375569250557 44.49107653816787z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M1321.852%2c371.041C1336.374%2c370.632%2c1351.171%2c365.909%2c1358.464%2c353.344C1365.782%2c340.737%2c1363.392%2c325.049%2c1355.757%2c312.631C1348.499%2c300.827%2c1335.697%2c294.381%2c1321.852%2c293.796C1306.752%2c293.158%2c1290.86%2c296.889%2c1282.588%2c309.537C1273.595%2c323.286%2c1272.648%2c341.662%2c1281.488%2c355.51C1289.802%2c368.533%2c1306.407%2c371.476%2c1321.852%2c371.041' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float1'%3e%3c/path%3e%3cpath d='M376.53195243191476 108.1968618135929L281.5421322424338 33.98268063509384 207.32795106393473 128.9725008245748 302.3177712534157 203.18668200307386z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float1'%3e%3c/path%3e%3cpath d='M654.5645974492476 523.6515117959083L634.5470780181092 410.12651777224926 541.0396034255886 543.6690312270466z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M479.2523320067578 71.24531480382576L501.1785109483603 195.59485480902012 603.6018720119522 49.31913586222324z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M1053.2541047205782 456.45353800140987L1104.0338795672703 588.7393741621404 1185.5399408813087 405.67376315471785z' fill='rgba(10%2c 123%2c 255%2c 0.3)' class='triangle-float3'%3e%3c/path%3e%3c/g%3e%3cdefs%3e%3cmask id='SvgjsMask1010'%3e%3crect width='1440' height='560' fill='white'%3e%3c/rect%3e%3c/mask%3e%3cstyle%3e %40keyframes float1 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-10px%2c 0)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float1 %7b animation: float1 5s infinite%3b %7d %40keyframes float2 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-5px%2c -5px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float2 %7b animation: float2 4s infinite%3b %7d %40keyframes float3 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(0%2c -10px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float3 %7b animation: float3 6s infinite%3b %7d %3c/style%3e%3c/defs%3e%3c/svg%3e");
}
</style>
