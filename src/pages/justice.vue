<template>
  <q-page
    class="flex flex-center items-stretch"
  >
    <div>
      <generic-header
        :image-src="HEADER[2].image"
        red-text="justice"
        white-text="ad"
        flip
        :description="HEADER[2].description"
      />
    </div>

    <div class="bg-white full-width seperator q-my-xl" />

    <generic-article
      :image-src="ARTICLE[2].image"
      :title="ARTICLE[2].title"
      :description1="ARTICLE[2].description1"
      :description2="ARTICLE[2].description2"
      :description3="ARTICLE[2].description3"
      :description4="ARTICLE[2].description4"
    />

    <div class="bg-white full-width seperator q-my-xl" />

    <generic-video
      :title="VIDEO[2].title"
      :description="VIDEO[2].description"
      :video-src="VIDEO[2].video"
      volume="1"
    />

    <div class="bg-white full-width seperator q-my-xl" />

    <generic-infographics
      :description="INFOGRAPHICS[2].description"
      :image-src="INFOGRAPHICS[2].image"
    />
  </q-page>
  <div class="bg-white full-width seperator q-my-xl" />
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import GenericHeader from 'src/components/GenericHeader.vue'
import GenericArticle from 'src/components/GenericArticle.vue'
import GenericVideo from 'src/components/GenericVideo.vue'
import GenericInfographics from 'src/components/GenericInfographics.vue'
import { HEADER, ARTICLE, VIDEO, INFOGRAPHICS } from 'src/components/constants'

const description = ref('Your hub for local justice advocacy in the Philippines. Stay informed about key issues, meet inspiring advocates, and join the movement for a fair and just society.')

</script>

<style scoped lang="sass">

</style>
