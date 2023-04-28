<template>
  <div class="page-section bg-pink-50">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 py-3 wow fadeInUp">
          <ul class="contact-list">
            <li>
              <lord-icon
                src="https://cdn.lordicon.com/qemhfpjm.json"
                trigger="hover"
                colors="primary:#121331,secondary:#b26836,tertiary:#4bb3fd,quaternary:#f9c9c0,quinary:#ebe6ef"
                stroke="15"
                state="hover-glance"
                style="width: 50px; height: 50px;"
              >
              </lord-icon>
              <div class="content">Николаева Ирина</div>
            </li>
            <li>
              <lord-icon
                src="https://cdn.lordicon.com/gzmgulpl.json"
                trigger="hover"
                colors="outline:#121331,primary:#4bb3fd,secondary:#ebe6ef"
                stroke="10"
                style="width: 50px; height: 50px;"
              >
              </lord-icon>
              <div class="content"><a href="#">Ksonra@mail.ru</a></div>
            </li>
            <li>
              <lord-icon
                src="https://cdn.lordicon.com/ovmtvwil.json"
                trigger="hover"
                colors="primary:#f9c9c0,secondary:#121331,tertiary:#66a1ee"
                stroke="15"
                style="width: 50px; height: 50px;"
              >
              </lord-icon>
              <div class="content"><a href="#">+375296411979</a></div>
            </li>
          </ul>
        </div>
        <div class="col-lg-6 py-3 wow fadeInUp">
          <div></div>
          <div></div>
          <div class="subhead">Свяжись со мной</div>
          <div class="divider"></div>
          <form action="#">
            <div class="py-2">
              <input type="text" class="form-control" placeholder="ФИО" />
            </div>
            <div class="py-2">
              <input type="text" class="form-control" placeholder="Email" />
            </div>
            <div class="py-2">
              <textarea
                rows="6"
                class="form-control"
                placeholder="Введите сообщение"
              ></textarea>
            </div>
            <div>
              <button
                type="submit"
                class="btn btn-outline-primary rounded-pill"
              >
                Отправить
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "./Navbar.vue";
import Footer from "./Footer.vue";

export default {
  name: "Contact",

  components: {
    Navbar: Navbar,
    Footer: Footer,
  },
};
</script>

<style></style>
