<script>
import Link from '@/components/Header/Link.vue'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  components: { Link, FontAwesomeIcon },
  name: 'IndexPage',
  data () {
    return {
    }
  }
}
</script>

<style>
  .gradient {
    @apply bg-gradient-to-br from-pacific-blue-600 to-pacific-blue-800;
  }

  .text-gradient {
    @apply bg-gradient-to-br from-pacific-blue-500 to-pacific-blue-900 bg-clip-text text-transparent;
  }
</style>

<template>
  <div class="h-full">
    <Nuxt />
    <div class="gradient py-3 px-5">
      <div class="max-w-[95%] md:max-w-7xl mx-auto md:block w-full md:w-auto md:flex-grow md:flex md:items-center">
        <ul class="hidden md:flex flex-col md:-mx-4 md:flex-row md:items-center md:mr-auto">
          <Link url="https://github.com/michaelbarrows" :target="() => '_blank'">
            <FontAwesomeIcon class="text-xl" :icon="['fab', 'github']" />
          </Link>
          <Link url="https://linkedin.com/in/michaelpbarrows" :target="() => '_blank'">
            <FontAwesomeIcon class="text-xl" :icon="['fab', 'linkedin']" />
          </Link>
        </ul>
        <p class="text-center md:text-right md:pl-10 text-white font-medium">&copy; Michael Barrows 2023</p>
      </div>
    </div>
  </div>
</template>
