
<template>
  <section>
    <Header />
    <Welcome />

    <Body />
    <Slider />
    <ContactUs />
    <Footer />
  </section>
</template>

<script>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";
import ContactUs from "../components/ContactUs.vue";
import Slider from "../components/Slider.vue";
import Welcome from "../components/Welcome.vue";
import Body from "../components/Body.vue";
export default {
  data() {
    return {
      slide: 0,
      sliding: null
    };
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true;
    },
    onSlideEnd(slide) {
      this.sliding = false;
    }
  },
  components: { Header, Footer, ContactUs, Slider, Welcome, Body }
}
</script>