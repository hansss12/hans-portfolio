<template>
  <Navbar />
  <div class="bg-green-50 page-section">
    <div class="container">
      <div class="row">
        <div
          class="relative col-md-6 col-lg-3 py-3 wow fadeInUp lg:hidden">
          <div class="bg-green-400 card-blog">
            <div class="header">
              <div class="entry-footer">
                <div class="post-author text-black text-lg">Certification</div>
                <a href="#" class="post-date"></a>
              </div>
            </div>
            <div class="body">
              <div class="post-title">
                <a>
                  My Knowledge
                  <br />
                  Research Skills
                  <br />
                  And License
                  <br />
                  Virtual Internship
                </a>
              </div>
            </div>
          </div>
        </div>

        <div v-for="(a, i) in blog" :key="a" class="col-md-6 col-lg-4 py-3">
          <div

            class="card-blog bg-white">
            <div class="header">
              <div class="avatar bg-white">
                <img :src="blog[i].profile" class="h-12 w-12"/>
              </div>
              <div class="entry-footer">
                <div class="font-semibold text-lg">{{ blog[i].username }}</div>
                <a class="post-date">{{ blog[i].date }}</a>
              </div>
            </div>

            <div class="body">
              <div class="post-title">
                <a>{{ blog[i].title }}</a>
              </div>
              <div class="post-excerpt">
                {{ blog[i].intro }}
              </div>
            </div>
            <div class="footer ml-2">
              <a :href="blog[i].link">
                Read More
                <span class="mai-chevron-forward text-sm"></span>
              </a>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>

  <Footer />
</template>

<script>
import Data from "../data/data.js";
import Navbar from "../components/Navbar";
import Footer from "../components/Footer";

export default {
  name: "Blog Page",
  data() {
    return {
      blog: Data,
    };
  },

  components: {
    Navbar,
    Footer,
  },
};
</script>

<style></style>
