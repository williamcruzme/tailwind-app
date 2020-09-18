<template>
  <div class="bg-gray-300">
    <!-- Your magic code here -->

    <section class="flex bg-gray-100">
      <div class="max-w-md px-8 py-12 mx-auto sm:max-w-xl lg:max-w-full lg:w-1/2 lg:py-24 lg:px-12">
        <div class="xl:max-w-lg xl:ml-auto">
          <img class="h-10" src="/img/workcation.svg" alt="Workcation">

          <!-- Card -->
          <img
            class="mt-6 rounded-lg shadow-xl sm:mt-8 sm:h-64 sm:w-full sm:object-cover sm:object-center lg:hidden"
            src="/img/beach-work.jpg"
            alt="Woman workcationing on the beach"
          >

          <h1 class="mt-6 text-2xl font-bold leading-tight text-gray-900 sm:mt-8 sm:text-4xl lg:text-3xl xl:text-4xl">
            You can work from anywhere.
            <br class="hidden lg:inline"><span class="text-indigo-500">Take advantage of it.</span>
          </h1>
          <p class="mt-2 text-gray-600 sm:mt-4 sm:text-xl">
            Workcation helps you find work-friendly rentals in beautiful locations so you can enjoy some nice weather even when you're not on vacation.
          </p>

          <!-- Actions -->
          <div class="mt-4 sm:mt-6">
            <button class="px-5 py-3 text-sm font-semibold tracking-wider text-white uppercase bg-indigo-500 rounded-lg shadow-lg hover:bg-indigo-400 active:bg-indigo-600 focus:outline-none focus:shadow-outline sm:text-base">
              Book your escape
            </button>
          </div>
        </div>
      </div>
      <div class="hidden lg:block lg:w-1/2 lg:relative">
        <img
          class="absolute inset-0 object-cover object-center w-full h-full"
          src="/img/beach-work.jpg"
          alt="Woman workcationing on the beach"
        >
      </div>
    </section>

    <!-- Your magic code here -->
  </div>
</template>
