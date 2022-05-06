<template>
  <div class="has-text-centered">
    <h2 class="title is-2 is-uppercase mb-5">
      Projets
    </h2>
    <div class="box">
      <p v-if="$fetchState.pending">Fetching mountains...</p>
      <p v-else-if="$fetchState.error">An error occurred :(</p>
      <b-loading v-model="isLoading" :is-full-page="false" />
      <div class="columns is-multiline">
        <div v-for="(mountain, key) of mountains" :key="key" class="column is-one-quarter">
          <div class="card">
            <header class="card-header">
              <p class="card-header-title">{{ mountain.title }}</p>
            </header>
            <div class="card-image">
              <figure class="image is-4by3">
                <img :src="mountain.image" :alt="mountain.title">
              </figure>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WebsitePresentation',
  data() {
    return {
      mountains: [],
      isLoading: false
    }
  },
  async fetch() {
    try {
      this.isLoading = true
      this.mountains = await fetch(
        'https://api.nuxtjs.dev/mountains'
      ).then(res => res.json())
      this.isLoading = false
    }
    catch (err) {
      console.log('err', err)
    }

  },
}
</script>
