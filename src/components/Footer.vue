<template>
  <footer class="page-footer">
    <div class="container">
      <div class="row justify-content-center mb-5">
        <div class="col-lg-3 py-3">
          <h3>My<span class="text-primary">Portfolio</span></h3>
          <p><a href="#">raihan.aqil2003@gmail.com</a></p>
          <p><a href="#">+62 812-2366-2003</a></p>
        </div>
        <div class="col-lg-3 py-3">
          <h5>Quick Links</h5>
          <ul class="footer-menu">
            <li class="nav-item active">
              <router-link to="/" class="nav-link">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">About</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/projects" class="nav-link"
                >Projects</router-link
              >
            </li>
            <li class="nav-item">
              <router-link to="/blog" class="nav-link">Certificate</router-link>
            </li>
          </ul>
        </div>
        <div class="col-lg-3 py-3">
          <h5>Certificate</h5>
            <ul class="footer-menu">
              <li class="nav-item" v-for="(B, i) in blog" :key="i">
                <a class="nav-link" :href="B.link">{{ B.username }}</a>
              </li>
            </ul>
        </div>
        <div class="col-lg-3 py-3">
          <h5>Subscribe</h5>
          <form action="#">
            <input
              type="text"
              class="form-control"
              placeholder="Enter your mail.."
            />
          </form>

          <div class="sosmed-button mt-4">
            <a href="#" class="mr-1">
              <span class="mai-logo-linkedin flex justify-center">
                <svg class="h-6 w-6 text-black relative top-2"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round">  <path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z" /></svg>
              </span>
            </a>
            <a href="https://www.instagram.com/raihann__12/" class="mr-1">
              <span class="mai-logo-linkedin flex justify-center">
                <svg class="h-6 w-6 text-black relative top-2"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round">  <rect x="2" y="2" width="20" height="20" rx="5" ry="5" />  <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z" />  <line x1="17.5" y1="6.5" x2="17.51" y2="6.5" /></svg>
              </span>
            </a>
            <a href="https://github.com/hansss12" class="mr-1">
              <span class="mai-logo-linkedin flex justify-center">
                <svg class="h-6 w-6 relative top-2 text-black"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round">  <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22" /></svg>
              </span>
            </a>
            <a href="https://www.linkedin.com/in/raihan-aqil-fadillah/" class="mr-1">
              <span class="mai-logo-linkedin flex justify-center">
                <svg class="h-6 relative top-2 w-6 text-black"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round">  <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z" />  <rect x="2" y="9" width="4" height="12" />  <circle cx="4" cy="4" r="2" /></svg>
              </span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </footer>
  <div
    class="lg:hidden fixed bottom-0 left-0 z-20 w-full rounded-t-xl drop-shadow-xl px-1 bg-gray-50 border-t border-gray-200 shadow md:flex md:items-center md:justify-between md:p-6 dark:bg-gray-800 dark:border-gray-600">
    <div>
      <div
        class="flex flex-wrap items-center justify-evenly p-1 space-x-5 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
        <router-link
          @click="isActive"
          to="/"
          class="flex flex-col items-center justify-center">
          <div
            class="flex items-center hover:no-underline mt-1 text-gray-900 rounded-lg dark:text-white hover:bg-blue-100 dark:hover:bg-gray-700"
            aria-current="page">
            <svg
              aria-hidden="true"
              class="flex-shrink-0 w-6 h-6 text-green-500 transition duration-75 hover:-mt-1 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg">
              <path
                clip-rule="evenodd"
                fill-rule="evenodd"
                d="M9.293 2.293a1 1 0 011.414 0l7 7A1 1 0 0117 11h-1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-3a1 1 0 00-1-1H9a1 1 0 00-1 1v3a1 1 0 01-1 1H5a1 1 0 01-1-1v-6H3a1 1 0 01-.707-1.707l7-7z"></path>
            </svg>
          </div>
          <div
            class="flex items-center justify-center mt-1 text-green-900 hover:no-underline font-medium rounded-lg dark:text-white dark:hover:bg-gray-700"
            aria-current="page">
            <p class="">Home</p>
          </div>
        </router-link>

        <router-link
          to="/projects"
          class="flex flex-col items-center justify-center">
          <div
            class="flex items-center hover:no-underline mt-1 text-gray-900 rounded-lg dark:text-white hover:bg-blue-100 dark:hover:bg-gray-700"
            aria-current="page">
            <svg
              aria-hidden="true"
              class="flex-shrink-0 w-6 h-6 text-green-500 transition duration-75 dark:text-gray-400 dark:group-hover:text-white"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg">
              <path
                d="M2 4.25A2.25 2.25 0 014.25 2h2.5A2.25 2.25 0 019 4.25v2.5A2.25 2.25 0 016.75 9h-2.5A2.25 2.25 0 012 6.75v-2.5zM2 13.25A2.25 2.25 0 014.25 11h2.5A2.25 2.25 0 019 13.25v2.5A2.25 2.25 0 016.75 18h-2.5A2.25 2.25 0 012 15.75v-2.5zM11 4.25A2.25 2.25 0 0113.25 2h2.5A2.25 2.25 0 0118 4.25v2.5A2.25 2.25 0 0115.75 9h-2.5A2.25 2.25 0 0111 6.75v-2.5zM15.25 11.75a.75.75 0 00-1.5 0v2h-2a.75.75 0 000 1.5h2v2a.75.75 0 001.5 0v-2h2a.75.75 0 000-1.5h-2v-2z"></path>
            </svg>
          </div>
          <div
            class="flex items-center justify-center mt-1 text-green-900 font-medium rounded-lg dark:text-white dark:hover:bg-gray-700"
            aria-current="page">
            <p class="whitespace-nowrap">Projects</p>
          </div>
        </router-link>
        <router-link
          to="/about"
          class="flex flex-col items-center justify-center">
          <div
            class="flex items-center hover:no-underline mt-1 text-gray-900 rounded-lg dark:text-white dark:hover:bg-gray-700"
            aria-current="page">
            <svg
              aria-hidden="true"
              class="flex-shrink-0 w-6 h-6 text-green-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg">
              <path
                clip-rule="evenodd"
                fill-rule="evenodd"
                d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"></path>
            </svg>
          </div>
          <div
            class="flex items-center justify-center mt-1 text-green-900 font-medium rounded-lg dark:text-white dark:hover:bg-gray-700"
            aria-current="page">
            <p class="whitespace-nowrap">About</p>
          </div>
        </router-link>
        <router-link
          to="/blog"
          class="flex flex-col items-center justify-center">
          <div
            class="flex items-center hover:no-underline hover:text-green-500 mt-1 text-gray-900 rounded-lg dark:text-white hover:bg-blue-100 dark:hover:bg-gray-700"
            aria-current="page">
            <svg
              aria-hidden="true"
              class="flex-shrink-0 w-6 h-6 text-green-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
              fill="currentColor"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg">
              <path
                clip-rule="evenodd"
                fill-rule="evenodd"
                d="M1 5.25A2.25 2.25 0 013.25 3h13.5A2.25 2.25 0 0119 5.25v9.5A2.25 2.25 0 0116.75 17H3.25A2.25 2.25 0 011 14.75v-9.5zm1.5 5.81v3.69c0 .414.336.75.75.75h13.5a.75.75 0 00.75-.75v-2.69l-2.22-2.219a.75.75 0 00-1.06 0l-1.91 1.909.47.47a.75.75 0 11-1.06 1.06L6.53 8.091a.75.75 0 00-1.06 0l-2.97 2.97zM12 7a1 1 0 11-2 0 1 1 0 012 0z"></path>
            </svg>
          </div>
          <div
            class="flex items-center justify-center mt-1 hover:text-green-500 text-green-900 font-medium rounded-lg dark:text-white hover:bg-blue-100 dark:hover:bg-gray-700"
            aria-current="page">
            <div class="whitespace-nowrap">Certificate</div>
          </div>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
import Data from "../data/data.js";

export default {
  data() {
    return {
      blog: Data,
    }
  },
};
</script>

<style></style>
