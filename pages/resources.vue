<template>
  <div class="bg-light-elevatedSurface dark:bg-dark-elevatedSurface shadow-nuxt transition-colors duration-300 ease-linear">
    <div class="container mx-auto px-4 pt-16">
      <div class="flex flex-wrap justify-between mb-8">
        <div class="lg:w-6/12 lg:text-left text-center p-4 sm:p-0">
          <h1 class="text-3xl xl:text-4xl text-light-onSurfacePrimary dark:text-dark-onSurfacePrimary font-medium leading-normal mb-6 lg:pt-4">
            NUXT<span class="text-primary-base">JS</span> Resources<br>
          </h1>
          <h3 class="xl:text-lg text-light-onSurfaceSecondary dark:text-dark-onSurfaceSecondary font-medium leading-relaxed mb-6">
            Discover a panel of resources made by our partners. By using thoses affiliate resources links, you are helping us to maintain and develop the Open Source Framework.
          </h3>
        </div>
        <i-themes class="w-2/3 mx-auto lg:mx-0 lg:w-5/12 lg:-mt-8 text-light-elevatedSurface dark:text-dark-elevatedSurface"/>
      </div>
      <section class="flex flex-wrap -mx-4">
        <nuxt-link :to="{ name: 'themes' }" class="block w-full lg:w-1/2 p-4">
          <div class="block bg-light-surface dark:bg-dark-surface hover:bg-gray-200 rounded p-8 text-center transition-colors duration-300 ease-linear">
            <h2 class="text-2xl text-light-onSurfacePrimary dark:text-dark-onSurfacePrimary font-medium uppercase mb-8 transition-colors duration-300 ease-linear">Themes</h2>
            <i-theming class="text-light-onSurfacePrimary dark:text-dark-onSurfacePrimary inline-block w-auto h-40 sm:h-56 xl:h-64 transition-colors duration-300 ease-linear"></i-theming>
          </div>
        </nuxt-link>
        <nuxt-link :to="{ name: 'video-courses' }" class="w-full lg:w-1/2 p-4">
          <div class="block bg-light-surface dark:bg-dark-surface hover:bg-gray-200 rounded p-8 text-center transition-colors duration-300 ease-linear">
            <h2 class="text-2xl text-light-onSurfacePrimary dark:text-dark-onSurfacePrimary font-medium uppercase mb-8 transition-colors duration-300 ease-linear">Video Courses</h2>
            <i-videos class="text-light-onSurfacePrimary dark:text-dark-onSurfacePrimary inline-block w-auto h-40 sm:h-56 xl:h-64 transition-colors duration-300 ease-linear"></i-videos>
          </div>
        </nuxt-link>
      </section>
    </div>
  </div>
</template>

<script>
import iThemes from '@/components/svg/fogg/themes'
import iTheming from '@/components/svg/fogg/theming'
import iVideos from '@/components/svg/fogg/videos'

export default {
  components: {
    iThemes,
    iTheming,
    iVideos
  },
  head: {
    title: 'NuxtJS Resources',
    meta: [
      { hid: 'description', name: 'description', content: 'Discover a panel of resources made by our partners. By using thoses affiliate resources links, you are helping us to maintain and develop the Open Source Framework.' }
    ]
  }
}
</script>
