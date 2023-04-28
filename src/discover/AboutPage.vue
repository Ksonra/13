<template>
  <Navbar />
  <div class="hidden lg:block container mt-5">
    <div class="page-banner1">
      <div class="row justify-content-center align-items-center h-100">
        <div class="col-md-6">
          <nav aria-label="Breadcrumb">
            <ul class="breadcrumb justify-content-center py-0 bg-transparent">
              <li class="breadcrumb-item">
                <router-link to="/">Домой</router-link>
              </li>
              <li class="breadcrumb-item active">Обо мне</li>
            </ul>
          </nav>
          <h1 class="text-center">Подробнее</h1>
        </div>
      </div>
    </div>
  </div>
  <About />
  <div class="bg-pink-50 py-5 page-section">
    <Contact />
  </div>

  <Footer :blog="blog" />
</template>

<script>
import Navbar from "../components/Navbar";
import About from "../components/About";
import Footer from "../components/Footer";
import Contact from "@/components/Contact.vue";

export default {
  name: "About Page",
  data() {
    return {};
  },

  props: {
    blog: Array,
  },

  components: {
    Navbar,
    About,
    Footer,
    Contact,
  },
};
</script>

<style></style>
