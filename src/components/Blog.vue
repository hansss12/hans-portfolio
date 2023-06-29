<template>
  <div class="bg-green-50 page-section py-5">
    <div class="container">
      <div class="text-center wow fadeInUp">
        <div class="mt-2 subhead">Certification</div>
        <h2 class="title-section">
          My latest
          <span class="">Certificate</span>
        </h2>
        <div class="divider mx-auto"></div>
      </div>

      <div class="row my-5 card-blog-row">
        <div class="col-md-6 col-lg-3 py-3 wow fadeInUp hover:-mt-3">
          <div class="card-blog">
            <div class="header">
              <div class="entry-footer">
                <div class="post-author">Certification</div>
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

        <div
          v-for="(a, i) in 3"
          :key="a"
          class="col-md-6 col-lg-3 py-3 wow fadeInUp hover:-mt-3">
          <div class="bg-white card-blog">
            <div class="header">
              <div class="avatar bg-white">
                <img :src="blog[i].profile" class="h-12 w-12"/>
              </div>
              <div class="entry-footer">
                <div class="font-semibold">{{ blog[i].username }}</div>
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
            <div class="footer">
              <a :href="blog[i].link">
                Read More
                <span class="mai-chevron-forward text-sm"></span>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="text-center pb-5">
        <a
          href="https://www.linkedin.com/in/raihan-aqil-fadillah/details/certifications/"
          class="btn btn-outline-primary rounded-pill">
          Discover More
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    blog: Array,
  },
};
</script>

<style></style>
