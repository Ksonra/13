<template>
  <Navbar />
  <Header />
  <About />

  <div class="bg-pink-50 py-5 page-section">
    <div class="container">
      <div class="text-center wow fadeInUp">
        <div class="text-2xl mb-3">Мои персональные преимущества</div>
        <div class="divider mx-auto"></div>
      </div>
      <div
        class="flex flex-col lg:flex-row items-center justify-evenly space-x-3 h-full text-left py-5"
      >
        <div
          class="bg-white rounded-xl drop-shadow-md mt-3 col-lg-4 ml-2 py-1 px-5 h-96 hover:-mt-3 cursor-default hover:shadow-lg hover:shadow-blue-100"
        >
          <lord-icon
            src="https://cdn.lordicon.com/hursldrn.json"
            trigger="hover"
            style="width: 150px; height: 150px;"
            class="hidden lg:flex"
          ></lord-icon>
          <div class="text-2xl font-semibold text-green-800 mt-4 pl-1">
            Самообучение
          </div>
          <p class="text-left text-base lg:text-sm leading-relaxed">
            Моя сила в желании находить ответы. Умение найти возможность для
            реализации задуманных планов.
          </p>
        </div>
        <div
          class="bg-white rounded-xl drop-shadow-md mt-3 col-lg-4 ml-2 py-1 px-5 h-96 hover:-mt-3 cursor-default hover:shadow-lg hover:shadow-blue-100"
        >
          <lord-icon
            src="https://cdn.lordicon.com/dfxesbyu.json"
            trigger="morph"
            style="width: 150px; height: 150px;"
            class="hidden lg:flex"
          ></lord-icon>

          <div class="text-2xl font-semibold text-green-800 mt-4 pl-1">
            Честность и самокритичность
          </div>
          <p class="text-left text-base lg:text-sm leading-relaxed">
            Важное качество для разработчика,
            научится признавать ошибки, устранять их и извлекать уроки на
            будущее.
          </p>
          <br />
          "Не ошибается тот, кто ничего не делает."
          <br>
          - Теодор Рузвельт
        </div>
      </div>
    </div>
    <div class="text-center pb-5">
        <router-link
          to="https://vueblog-13514.web.app/"
          class="btn btn-outline-primary rounded-pill">
          Продолжить
        </router-link>
      </div>
  </div>

  <Blog :blog="blog" />
  <Footer />
</template>

<script>
import Navbar from "./Navbar.vue";
import Header from "./Header.vue";
import About from "./About.vue";
import Projects from "./Projects.vue";
import Contact from "./Contact.vue";
import Footer from "./Footer.vue";

export default {
  name: "Home",
  data() {
    return {};
  },

  props: {
    blog: Array,
  },

  components: {
    Navbar,
    Header,
    About,
    Projects,
    Contact,
    Footer,
  },
};
</script>

<style></style>
