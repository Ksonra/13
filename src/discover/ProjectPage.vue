<template>
  <Navbar />
  <div>
    <div class="hidden lg:block container">
      <div class="page-banner1 bg-pink-50">
        <div class="row justify-content-center align-items-center h-80">
          <div class="col-md-6">
            <nav aria-label="Breadcrumb">
              <ul class="breadcrumb justify-content-center py-0 bg-transparent">
                <li class="breadcrumb-item">
                  <router-link to="/">Домой</router-link>
                </li>
                <li class="breadcrumb-item active">Проекты</li>
              </ul>
            </nav>
            <p class="text-center text-2xl font-semibold marked">
              <span class="marked">Мои будущие проекты</span>
            </p>
            <div class="divider mx-auto"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-section bg-pink-50">
      <div class="container">
        <div class="row my-5 card-blog-row">
          <div
            v-for="(a, i) in project"
            :key="a"
            class="col-md-5 col-lg-4 py-5 px-4"
          >
            <div
              class="flex flex-col space-y-5 border shadow-md border-blue-500 bg-white h-96 rounded-md hover:-mt-1 hover:shadow-lg hover:shadow-blue-200 cursor-pointer"
            >
              <div
                class="flex items-center justify-center -mt-6 h-48 rounded-t-lg overflow-hidden"
              >
                <img class="rounded-t-lg" :src="project[i].image" />
              </div>

              <div class="flex flex-col ml-4">
                <div class="text-xl font-medium text-blue-600 ml-3 mb-2">
                  <a>{{ project[i].name }}</a>
                </div>
                <div
                  class="text-base h-18 lg:h-12 text-gray-700 ml-3 mr-3 mb-2"
                >
                  {{ project[i].content }}
                </div>

                <div
                  class="flex flex-row items-center justify-center py-3 px-2 space-x-3 ml-2"
                  style="padding-bottom: 25px;"
                >
                  <img :src="project[i].tech1" />
                  <img :src="project[i].tech2" />
                </div>
              </div>
            </div>
            <div class="flex items-center justify-center mt-4 hover:underline">
              <router-link
                to="https://vueblog-13514.web.app/"
                class="btn btn-primary"
              >
                Посмотреть код
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProjectData from "../data/projects.js";
import Navbar from "../components/Navbar";

export default {
  name: "Project Page",
  data() {
    return {
      project: ProjectData,
    };
  },
  props: {
    blog: Array,
  },
  components: { Navbar },
};
</script>

<style></style>
