<template>
  <main class="antialiased">
    <!-- Navbar small (logo only) -->
    <div class="flex items-center justify-center pt-5 md:hidden">
      <img class="h-5" src="/img/vercel.svg" alt="Vercel">
    </div>

    <!-- Navbar -->
    <nav class="items-center justify-between hidden max-w-5xl px-5 mx-auto my-4 font-sans md:flex">
      <!-- Left navbar -->
      <div class="flex items-center justify-start w-1/3">
        <img class="h-6" src="/img/vercel.svg" alt="Vercel">
      </div>

      <!-- Center navbar -->
      <div class="flex items-center justify-center w-1/3 font-light text-gray-700">
        <span class="flex items-center mx-2">
          Solutions <ChevronDown class="w-3 ml-1" />
        </span>
        <span class="flex items-center mx-2">
          Resources <ChevronDown class="w-3 ml-1" />
        </span>
        <span class="flex items-center mx-2">
          Pricing
        </span>
      </div>

      <!-- Right navbar -->
      <div class="flex items-center justify-end w-1/3">
        <TheButton>
          Contact
        </TheButton>
        <TheButton>
          Login
        </TheButton>
        <TheButton primary>
          Sign Up
        </TheButton>
      </div>
    </nav>

    <!-- Content -->
    <div class="py-8">
      <div
        ref="dspContainer"
        class="flex flex-col items-center justify-center mb-12 text-6xl font-extrabold leading-tight tracking-tighter font-inter md:text-7xl"
      >
        <GradientText from="from-blue-600" to="to-teal-400" :style="{ bottom: '-0.2em' }">
          Develop.
        </GradientText>
        <GradientText from="from-purple-600" to="to-pink-600">
          Preview.
        </GradientText>
        <GradientText from="from-red-600" to="to-yellow-500" :style="{ top: '-0.2em' }">
          Ship.
        </GradientText>
      </div>

      <div class="flex items-center justify-center max-w-4xl mx-auto mb-16">
        <button class="w-48 py-3 mx-2 text-white bg-black rounded-md">
          Start Deploying
        </button>
        <button class="w-48 py-3 mx-2 font-medium text-gray-700 border border-gray-400 rounded-md">
          Get a Demo
        </button>
      </div>

      <div class="max-w-4xl px-5 mx-auto mb-12 text-center">
        <p class="text-lg text-gray-700">
          Vercel combines the best developer experience with an obsessive
          focus on end-user performance. Our platform enables frontend teams
          to do their best work.
        </p>
      </div>
    </div>
  </main>
</template>

<script>
import { TimelineMax } from 'gsap'
import ChevronDown from '~/assets/icons/chevron-down.svg?inline'

export default {
  components: {
    ChevronDown
  },
  mounted () {
    const dspContainer = this.$refs.dspContainer
    const tl = new TimelineMax({ repeat: -1 })
    const tween = {
      css: {
        color: 'transparent'
      },
      repeat: 1,
      yoyo: true
    }

    for (let i = 0; i < dspContainer.children.length; i++) {
      tl.to(dspContainer.children[i], 1.2, tween)
    }
  }
}
</script>
