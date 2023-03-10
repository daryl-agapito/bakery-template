<script>
export default {
  props: ['imageLink', 'title', 'description']
}
</script>

<script setup>
const fileUrl = new URL(`/src/assets/images/hc-1.jpg`, import.meta.url)
</script>

<template>
  <div
    class="card h-96 md:max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
  >
    <a href="#">
      <img class="rounded-lg card_img" :src="imageLink" alt="" />
    </a>
    <div class="read_more w-full absolute bottom-0 assign-center flex flex-col text-center">
      <div class="icons absolute">
        <a
          href="#"
          class="inline-flex items-center px-3 py-3 text-sm font-medium text-center text-white bg-blue-700 rounded-full hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          <svg
            fill="none"
            stroke="currentColor"
            stroke-width="1.5"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
            aria-hidden="true"
            class="w-5 h-5"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
            ></path>
          </svg>
        </a>
      </div>

      <div class="card_text p-5 py-8">
        <a href="#">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
            {{ title }}
          </h5>
        </a>

        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
          {{ description }}
        </p>
      </div>
    </div>
  </div>
</template>
