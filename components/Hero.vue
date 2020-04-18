<template>
  <section class="relative bg-white overflow-hidden">
    <div class="hidden lg:block lg:absolute lg:inset-0">
      <svg
        class="absolute top-0 left-1/2 transform translate-x-64 -translate-y-8"
        width="640"
        height="784"
        fill="none"
        viewBox="0 0 640 784"
      >
        <defs>
          <pattern
            id="9ebea6f4-a1f5-4d96-8c4e-4c2abf658047"
            x="118"
            y="0"
            width="20"
            height="20"
            patternUnits="userSpaceOnUse"
          >
            <rect
              x="0"
              y="0"
              width="4"
              height="4"
              class="text-gray-200"
              fill="currentColor"
            />
          </pattern>
        </defs>
        <rect
          y="72"
          width="640"
          height="640"
          class="text-gray-50"
          fill="currentColor"
        />
        <rect
          x="118"
          width="404"
          height="784"
          fill="url(#9ebea6f4-a1f5-4d96-8c4e-4c2abf658047)"
        />
      </svg>
    </div>
    <div class="relative pt-6 pb-16 md:pb-20 lg:pb-24 xl:pb-32">
      <nav
        class="relative max-w-screen-xl mx-auto flex items-center justify-between px-4 sm:px-6"
      >
        <div class="flex items-center flex-1">
          <div class="flex items-center justify-between w-full md:w-auto">
            <a href="#">
              <img
                class="h-8 w-auto sm:h-10"
                src="~/assets/logo.svg"
                alt="Logo"
              />
            </a>
            <div class="-mr-2 flex items-center md:hidden">
              <button
                @click="open = true"
                type="button"
                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out"
              >
                <svg
                  class="h-6 w-6"
                  stroke="currentColor"
                  fill="none"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M4 6h16M4 12h16M4 18h16"
                  />
                </svg>
              </button>
            </div>
          </div>
          <div class="hidden md:block md:ml-10">
            <a
              href="#"
              class="font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
              >Our values</a
            >
            <a
              href="#"
              class="ml-10 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
              >The tours</a
            >
            <a
              href="#"
              class="ml-10 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
              >Meet the guides</a
            >
          </div>
        </div>
        <div class="hidden md:block text-right">
          <span class="inline-flex rounded-md shadow-md">
            <span class="inline-flex rounded-md shadow-xs">
              <button
                type="button"
                class="inline-flex items-center px-4 py-2 leading-6 font-medium rounded-md text-gray-50 bg-green-600 hover:bg-green-500 focus:outline-none focus:shadow-outline-green transition duration-150 ease-in-out"
              >
                <img
                  src="~/assets/icons/whatsapp.svg"
                  alt=""
                  class="mr-2 h-4 w-auto sm:h-6"
                />
                Book a tour
              </button>
            </span>
          </span>
        </div>
      </nav>

      <div class="md:hidden">
        <transition
          enter-active-class="duration-150 ease-out"
          enter-class="opacity-0 scale-95"
          enter-to-class="opacity-100 scale-100"
          leave-active-class="duration-100 ease-in"
          leave-class="opacity-100 scale-100"
          leave-to-class="opacity-0 scale-95"
        >
          <div
            v-show="open"
            class="z-10 absolute top-0 inset-x-0 p-2 transition transform origin-top-right"
          >
            <div class="rounded-lg shadow-md">
              <div class="rounded-lg bg-white shadow-xs overflow-hidden">
                <div class="px-5 pt-4 flex items-center justify-between">
                  <div class="-mr-2">
                    <button
                      @click="open = false"
                      class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out"
                    >
                      <svg
                        class="h-6 w-6"
                        stroke="currentColor"
                        fill="none"
                        viewBox="0 0 24 24"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M6 18L18 6M6 6l12 12"
                        />
                      </svg>
                    </button>
                  </div>
                </div>
                <div class="px-2 pt-2 pb-3">
                  <a
                    href="#"
                    class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                    >Our values</a
                  >
                  <a
                    href="#"
                    class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                    >The tours</a
                  >
                  <a
                    href="#"
                    class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                    >Meet the guides</a
                  >
                </div>
                <div>
                  <button
                    type="button"
                    class="flex justify-center items-center w-full px-5 py-3 text-lg font-medium text-gray-50 bg-green-600 hover:bg-green-500 focus:outline-none focus:shadow-outline-green transition duration-150 ease-in-out"
                  >
                    <img
                      src="~/assets/icons/whatsapp.svg"
                      alt=""
                      class="mr-2 h-6 w-auto sm:h-8"
                    />
                    Book a tour
                  </button>
                </div>
              </div>
            </div>
          </div>
        </transition>
      </div>

      <div
        class="mt-8 mx-auto max-w-screen-xl px-4 sm:mt-12 sm:px-6 md:mt-20 xl:mt-24"
      >
        <div class="lg:grid lg:grid-cols-12 lg:gap-8">
          <div
            class="sm:text-center md:max-w-2xl md:mx-auto lg:col-span-6 lg:text-left"
          >
            <h2
              class="mt-1 text-4xl tracking-tight leading-10 font-extrabold text-gray-700 sm:leading-none sm:text-6xl lg:text-5xl xl:text-6xl"
            >
              Ho Chi Minh City
              <br class="inline" />
              <span
                :class="{
                  'text-teal-400': color === 'teal',
                  'text-pink-400': color === 'pink',
                  'text-red-400': color === 'red'
                }"
                >{{ info('title') }}</span
              >
            </h2>
            <div class="px-8 sm:px-4 mt-8 sm:mt-12">
              <p
                class="text-base text-gray-500 sm:text-xl lg:text-lg xl:text-xl quote"
              >
                {{ info('quote') }} — <b>Anthony Bourdain</b>
              </p>
            </div>
          </div>
          <div
            class="mt-12 relative sm:max-w-lg sm:mx-auto lg:mt-0 lg:max-w-none lg:mx-0 lg:col-span-6 lg:flex lg:items-center"
          >
            <div
              class="overflow-hidden w-full shadow-2xl rounded-lg layer"
              :class="{
                'bg-teal-200': color === 'teal',
                'bg-pink-200': color === 'pink',
                'bg-red-200': color === 'red'
              }"
            >
              <img
                :src="info('image')"
                :alt="info('alt')"
                class="z-10 w-full h-full object-cover image"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      open: false,
      timerID: null,
      index: 2,
      information: [
        {
          color: 'pink',
          title: 'for the romantic',
          quote:
            "This is the way so many great meals in my life have been enjoyed: sitting in the street, eating something out of a bowl that I'm not exactly sure what it is, scooters going by. It's so delicious, I feel like an animal.",
          image: require('~/assets/images/church.jpg'),
          alt: 'Famous pink church in Saigon'
        },
        {
          color: 'red',
          title: 'for the adventurous',
          quote:
            'One of the great joys of life is riding a scooter through Vietnam, to be part of this mysterious, thrilling, beautiful choreography. Thousands upon thousands of people — families, friends, lovers — each an individual story glimpsed for a second or two in passing, sliding alongside, pouring like a torrent through the city. A flowing, gorgeous thing.',
          image: require('~/assets/images/adventure.jpg'),
          alt: 'Ho Chi Minh City popular area at night'
        },
        {
          color: 'teal',
          title: 'for the foodies',
          quote:
            'People are put on earth for various purposes; I was put on earth to do this. Eat noodles right here.',
          image: require('~/assets/images/food.jpg'),
          alt: 'Pho, the famous Vietnamese dish'
        }
      ]
    }
  },
  mounted() {
    this.timerID = setInterval(() => {
      this.index = (this.index + 1) % this.information.length
    }, 5000)
  },
  computed: {
    color() {
      return this.information[this.index].color
    }
  },
  methods: {
    info(field) {
      return this.information[this.index][field]
    }
  },
  beforeDestroy() {
    clearInterval(this.timerID)
  }
}
</script>

<style scoped>
.layer {
  height: 250px;
}

@screen lg {
  .layer {
    height: 400px;
  }
}

.image {
  mix-blend-mode: multiply;
}

.quote::before {
  content: '\201C';

  @apply absolute top-0 left-0 text-6xl -mt-8 -ml-8;
}

.quote {
  @apply relative inline;
}

.quote::after {
  content: '\201D';

  @apply absolute bottom-0 right-0 text-6xl -mb-16 -mr-8;
}
</style>