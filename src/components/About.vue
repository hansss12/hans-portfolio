<template>
  <div class="bg-green-50 page-section pt-5 -mb-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
          <div class="img-place text-center hidden lg:flex">
            <lottie-player
              src="https://assets2.lottiefiles.com/packages/lf20_qhrndegx.json"
              background="transparent"
              speed="1"
              style="max-width: 500px; max-height: 500px"
              autoplay></lottie-player>
          </div>
        </div>

        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            All About
            <span class="marked">Myself</span>
          </h2>
          <div class="divider"></div>

          <div>
            <p>
              I’m a Junior Fullstack Developer located in South jakarta, Indonesia.
              I learn a serious passion for UI effects,animations and creating intuitive,
              dynamic user experiences.
            </p>
          </div>

          <div>
            <p>
              I'm a well organized person, problem solver, independent employee
              with high attention to detail. Fan of Football, outdoor
              activities with my friends, TV series, Movies and English literature.
              Actually, I can be relocate at any place in java, indonesia
            </p>
          </div>

          <div>
            <p class="hidden lg:flex">
              And I'm interested in the entire creative frontend spectrum and
              working on ambitious projects with positive people.
            </p>
          </div>

          <div class="img-place mb-3"></div>
          <a href="#" class="btn btn-primary">More Details</a>
          <a href="#" class="btn btn-outline border ml-2">Success Stories</a>
        </div>
      </div>
    </div>
    <!-- .container -->
  </div>
  <!-- .page-section -->

  <div class="bg-green-50 page-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 p-4 -mt-9 lg:mt-0">
          <h2 class="title-section text-2xl">
            My
            <span class="marked">Skills & Experiences</span>
          </h2>
          <div class="divider"></div>
          <p class="mb-4">
            I graduated from Bootcamp Hacktiv8 Indonesia at 12 may 2023 with 
            predicate as Honors Awards and grade 93.1/100. My experiences in bootcamp 
            gave me strong communication and networking skills, which are crucial for
            event planning.
          </p>
          <p class="mb-4">
            I create successful responsive websites that are fast, easy to use,
            and built with best practices. The main area of my expertise is 
            Fullstack Developer with skills HTML, CSS, JS, with other javascript 
            framework like Vue js and React Js as Front end,
            as Back End i usualy use Node.js, Express, JWT and other programming language
            like phyton typescript and java, building small and simple web
            apps, features, animations, and coding interactive.
          </p>

          <router-link to="/blog" class="btn btn-primary mt-10">My Certificate</router-link>
          <router-link to="/projects" class="btn btn-outline ml-2 mt-10">
            My Projects
          </router-link>
        </div>
        <div class="col-lg-6 py-3 wow zoomIn">
          <div class="img-place text-center">
            <lottie-player
              src="https://assets2.lottiefiles.com/packages/lf20_u4jjb9bd.json"
              background="transparent"
              speed="0.5"
              style="max-width: 550px; max-height: 550px"
              loop
              autoplay></lottie-player>
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
