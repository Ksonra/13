<template>
  <div class="bg-pink-50 page-section pt-5 -mb-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
          <div class="img-place text-center hidden lg:flex">
            <lottie-player
              src="https://assets8.lottiefiles.com/packages/lf20_2t5zvcho.json"
              background="transparent"
              speed="1"
              style="max-width: 500px; max-height: 500px;"
              autoplay
            ></lottie-player>
          </div>
        </div>

        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            Все
            <span class="marked">обо мне</span>
          </h2>
          <div class="divider"></div>
          <div>
            <p>
              Привет, IT-мир! Сегодня день, когда мы наконец-то познакомимся...
              Итак, меня зовут Ирина и я делаю свой не первый, но от этого не
              менее волнительный, шаг в IT индустрию в качестве Full Stack
              Developer.
            </p>
          </div>
          <div>
            <p>
              Весьма самоорганизована, педантична и уделяю много внимания
              деталям. В свободное время увлекаюсь русским бильярдом и чтением
              художественной литературы.
            </p>
          </div>
          <router-link
              to="/about"
              name="fade"
              class="btn btn-primary"
            >
              Побробнее
            </router-link>
          </div>
      </div>
    </div>
  </div>
  <div class="bg-pink-60 page-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">
            Мои 
            <span class="marked">навыки</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            На данный момент, я- студентка БГУИР ИИТ по специальности Web-дизайн
            и компьютерная графика, по окончании которого будет присвоена
            квалификация – «Программист – Web-дизайнер»;
          </p>
          <p class="mb-4">
            Я работаю над созданием адаптивных веб-сайтов, быстрых и простых в
            использовании. Основная область моих знаний — разработка интерфейса
            ( Photoshop, Illustrator, 3D Max, Figma), HTML, CSS, JS, создание
            небольших и простых веб-приложений, анимаций и шаблонов.
          </p>

          <router-link to="/blog" class="btn btn-primary">Мои проекты</router-link>

        </div>
        <div class="col-lg-6 py-3 wow zoomIn">
          <div class="img-place text-center">
            <lottie-player
              src="https://assets2.lottiefiles.com/packages/lf20_u4jjb9bd.json"
              background="transparent"
              speed="0.5"
              style="max-width: 550px; max-height: 550px;"
              loop
              autoplay
            ></lottie-player>
          </div>
        </div>
      </div>
    </div>
    <!-- .container -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      scrollPosition: 0,
    };
  },

  methods: {
    handleScroll(e) {
      this.scrollPosition = e.target.scrollTop;

      if (this.scrollPosition > 100) {
        console.log("UP");
      } else {
        console.log("DOWN");
      }
    },
  },
};
</script>

<style></style>
