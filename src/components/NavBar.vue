<template>
  <header
    class="bg-gray-900 sm:flex sm:justify-between sm:items-center sm:px-4 sm:py-3"
  >
    <div class="flex items-center justify-between px-4 py-3 sm:p-0">
      <div>
        <img class="h-8" src="../assets/logo.png" alt="URecommend" />
      </div>
      <div class="sm:hidden">
        <button
          @click="isOpen = !isOpen"
          type="button"
          class="block py-1 text-white hover:text-white focus:text-white focus:outline-none"
        >
          <svg class="h-7 w-7 fill-current" viewBox="1 1 18 18" width="40">
            <path
              v-if="isOpen"
              fill-rule="evenodd"
              d="M10.185,1.417c-4.741,0-8.583,3.842-8.583,8.583c0,4.74,3.842,8.582,8.583,8.582S18.768,14.74,18.768,10C18.768,5.259,14.926,1.417,10.185,1.417 M10.185,17.68c-4.235,0-7.679-3.445-7.679-7.68c0-4.235,3.444-7.679,7.679-7.679S17.864,5.765,17.864,10C17.864,14.234,14.42,17.68,10.185,17.68 M10.824,10l2.842-2.844c0.178-0.176,0.178-0.46,0-0.637c-0.177-0.178-0.461-0.178-0.637,0l-2.844,2.841L7.341,6.52c-0.176-0.178-0.46-0.178-0.637,0c-0.178,0.176-0.178,0.461,0,0.637L9.546,10l-2.841,2.844c-0.178,0.176-0.178,0.461,0,0.637c0.178,0.178,0.459,0.178,0.637,0l2.844-2.841l2.844,2.841c0.178,0.178,0.459,0.178,0.637,0c0.178-0.176,0.178-0.461,0-0.637L10.824,10z"
              stroke-width="1"
              stroke="#C0C0C0"
            />
            <path
              v-if="!isOpen"
              fill-rule="evenodd"
              d="M10,1.445c-4.726,0-8.555,3.829-8.555,8.555c0,4.725,3.829,8.555,8.555,8.555c4.725,0,8.555-3.83,8.555-8.555C18.555,5.274,14.725,1.445,10,1.445 M10,17.654c-4.221,0-7.654-3.434-7.654-7.654c0-4.221,3.433-7.654,7.654-7.654c4.222,0,7.654,3.433,7.654,7.654C17.654,14.221,14.222,17.654,10,17.654 M14.39,10c0,0.248-0.203,0.45-0.45,0.45H6.06c-0.248,0-0.45-0.203-0.45-0.45s0.203-0.45,0.45-0.45h7.879C14.187,9.55,14.39,9.752,14.39,10 M14.39,12.702c0,0.247-0.203,0.449-0.45,0.449H6.06c-0.248,0-0.45-0.202-0.45-0.449c0-0.248,0.203-0.451,0.45-0.451h7.879C14.187,12.251,14.39,12.454,14.39,12.702 M14.39,7.298c0,0.248-0.203,0.45-0.45,0.45H6.06c-0.248,0-0.45-0.203-0.45-0.45s0.203-0.45,0.45-0.45h7.879C14.187,6.848,14.39,7.051,14.39,7.298"
              stroke="#C0C0C0"
              stroke-width="1"
              stroke-linecap="round"
            />
          </svg>
        </button>
      </div>
    </div>
    <nav :class="isOpen ? 'block' : 'hidden'" class="sm:block">
      <div class="px-2 pt-2 sm:flex">
        <a
          href="#"
          class="block px-2 py-1 text-white text-left font-semibold rounded hover:bg-gray-800"
          >List U Recommend</a
        >
        <a
          href="#"
          class="mt-1 block px-2 py-1 text-white text-left font-semibold rounded hover:bg-gray-800 sm:mt-0 sm:ml-2"
          >Configuration</a
        >
        <a
          href="#"
          class="mt-1 block px-2 py-1 text-white text-left font-semibold rounded hover:bg-gray-800 sm:mt-0 sm:ml-2"
          >Exit</a
        >
        <Account class="hidden sm:block sm:ml-6" />
      </div>

      <div class="px-4 py-5 mt-2 border-t border-gray-800 sm:hidden">
        <div class="flex items-center">
          <img
            class="h-8 w-8 border-2 border-gray-600 rounded-full object-cover"
            src="../assets/god.png"
            alt="your avatar"
          />
          <span class="ml-3 font-semibold text-white">Keanu Reeves</span>
        </div>
        <div class="mt-4">
          <a href="#" class="block text-gray-400 text-left hover:text-white"
            >Account settings</a
          >
          <a
            href="#"
            class="mt-2 block text-gray-400 text-left hover:text-white"
            >Support</a
          >
          <a
            href="#"
            class="mt-2 block text-gray-400 text-left hover:text-white"
            >Sign out</a
          >
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
import Account from "@/components/AccountDropDown.vue";

export default {
  components: {
    Account
  },
  name: "NavBar",
  data() {
    return {
      isOpen: false
    };
  }
};
</script>

<style></style>
