<template>
  <q-page class="">
    <section class="hero-wrapper">
      <div class="hero-layer1">
        <h1
          class="page-title text-left"
          data-aos="zoom-in"
          data-aos-delay="500"
        >
          Empowering <br />
          every aspect <br />of your business.
        </h1>
        <p class="page-caption">
          Boost productivity, explore fresh revenue opportunities and easily
          offer your services and accept bookings from anywhere.
          <br />
        </p>
        <q-btn
          size="lg"
          unelevated
          rounded
          color="primary"
          href=""
          no-wrap
          target="_blank"
          no-caps
          class="primary-btn q-my-sm"
          label="Get started - Join the Beta"
        />
      </div>
      <div class="hero-layer2 gt-sm">
        <!-- <img src="../assets/hero-star.svg" alt="" /> -->
      </div>
    </section>
    <section class="home-wrapper-two q-pa-md">
      <!-- <div class="row justify-between items-baseline q-mb-lg">
        <div class="col-12 col-md-6">
          <div class="wrapper-header">Services you need everyday</div>
        </div>
        <div class="col-12 col-md-6">
          <div class="wrapper-header-side">
            We packed together services you need at a cheaper than usual rate
          </div>
        </div>
      </div> -->
      <!-- <div class="row justify-between q-col-gutter-lg items-baseline q-mb-lg">
        <div class="col-12 col-md-6 text-center q-pa-md">
          <div>
            <q-img src="../assets/Mask1.svg" alt="" />
          </div>

          <div class="text-center q-mb-lg">
            <h3 class="mask-header">Mobile, Airtime & Data</h3>
            <div class="mask-description">
              Buy your data from Bonbonpay and airtime and <br />
              stay connected anytime, anywhere
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 text-center q-pa-md">
          <div>
            <q-img src="../assets/Mask2.svg" alt="" />
          </div>

          <div class="text-center q-mb-lg">
            <h3 class="mask-header">Electricity</h3>
            <div class="mask-description">
              Power Up Your Life with Easy and Convenient <br />
              Electricity Purchases on Bonbonpay
            </div>
          </div>
        </div>
      </div> -->
      <!-- <div class="row justify-between q-col-gutter-lg items-baseline">
        <div class="col-12 col-md-6 text-center q-pa-md">
          <div>
            <q-img src="../assets/Mask3.svg" alt="" />
          </div>

          <div class="text-center q-mb-lg">
            <h3 class="mask-header">Cable Subscriptions</h3>
            <div class="mask-description">
              Never Miss a Moment with Seamless Cable <br />
              Subscription Purchasing on Bonbonpay
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 text-center q-pa-md">
          <div>
            <q-img src="../assets/Mask4.svg" alt="" />
          </div>

          <div class="text-center q-mb-lg">
            <h3 class="mask-header">Waterbuy</h3>
            <div class="mask-description">
              Stay Hydrated with Hassle-Free Water Refill <br />
              Purchases on Bonbonpay
            </div>
          </div>
        </div>
      </div> -->
    </section>
    <section class="home-wrapper-two q-pa-md q-pt-lg" id="about">
      <div class="row justify-between q-my-lg q-py-lg">
        <div class="col-12 col-md-8 q-px-lg">
          <div
            class="wrapper-three-header q-mb-lg q-pb-lg"
            style="max-width: 760px"
          >
            Optimize your operations with: booking system, queue management,
            payroll, inventory management
          </div>
          <div
            class="mask-header mask-header2 q-pt-lg q-mt-lg"
            style="max-width: 760px"
          >
            We are a fintech startup aiming to deliver an all-in-one platform
            that seamlessly connects businesses with their clients, providing
            hassle-free booking and payment services. Our platform also offers
            smart tools that empower salons to manage their businesses more
            effectively, and drive growth with ease.
          </div>
        </div>
        <div class="col-12 col-md-4 q-pa-lg">
          <!-- <q-img src="../assets/Mask5.png" /> -->
        </div>
      </div>
    </section>
    <!-- <section class="q-py-lg q-px-md">
      <div class="full-width row justify-between items-stretch content-stretch">
        <div
          class="col-12 col-md-6 q-pl-lg gt-sm"
          style="border-radius: 100%; background: #2d5bff; position: relative"
        >
          <div class="child q-pl-lg q-ml-lg">
            <h2 class="wrapper-three-header text-white">
              Bonbonpay for <br />
              Android and iOS
            </h2>
            <p
              style="
                font-weight: 500;
                font-size: 20px;
                line-height: 30px;
                letter-spacing: -0.8px;
                opacity: 0.5;
              "
              class="text-white"
            >
              Stay Informed, Stay Ahead with Our Newsletter Subscription
            </p>
            <q-form
              @submit.prevent="submitForm"
              @reset="onReset"
              class="q-gutter-md"
            >
              <q-input
                v-model="email"
                class="text-secondary"
                color="secondary"
                type="email"
                label="Email"
              >
                <template v-slot:append>
                  <q-btn
                    rounded
                    flat
                    label="Send"
                    @click="submitForm"
                    color="secondary"
                    no-caps
                  />
                </template>
              </q-input>
            </q-form>
          </div>
        </div>
        <div class="col-12 col-md-6">
          <q-img src="../assets/Mask6.svg" />
        </div>
      </div>
    </section> -->
    <footer>
      <div class="row justify-between q-py-lg q-px-md">
        <p class="fw-500">All rights reserved.</p>
        <p class="fw-500">Contact us - hello@qtrim.com</p>
      </div>
    </footer>
  </q-page>
</template>

<script lang="ts">
import { Todo, Meta } from 'components/models';
import { defineComponent, ref } from 'vue';
import { useQuasar } from 'quasar';
export default defineComponent({
  name: 'IndexPage',
  setup() {
    const $q = useQuasar();
    const todos = ref<Todo[]>([
      {
        id: 1,
        content: 'ct1',
      },
      {
        id: 2,
        content: 'ct2',
      },
      {
        id: 3,
        content: 'ct3',
      },
      {
        id: 4,
        content: 'ct4',
      },
      {
        id: 5,
        content: 'ct5',
      },
    ]);
    const email = ref('');
    const meta = ref<Meta>({
      totalCount: 1200,
    });
    const submitForm = async () => {
      console.log(email.value);
      const data = {
        email: email.value,
      };
      fetch('https://formspree.io/f/xrgvkank', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(data),
      })
        .then((res) => res.json())
        .then((data) => {
          console.log(data);
          $q.notify({
            message: 'Thanks for subscribing to our Newsletter',
            type: 'positive',
          });
        });
      email.value = '';
    };
    const onReset = () => {
      email.value = '';
    };

    return { todos, meta, email, submitForm, onReset };
  },
});
</script>
<style>
.child {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}
.fw-500 {
  font-weight: 500;
}
</style>
