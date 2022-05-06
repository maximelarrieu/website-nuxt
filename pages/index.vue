<template>
  <section class="section has-text-centered">
    <h1 class="title is-1 is-uppercase">Maxime Larrieu</h1>
    <font-awesome-icon icon="['fab', 'facebook']"  style="font-size: 22px"/>
    <b-button
      label="Consultez mon CV"
      type="is-primary"
      size="is-medium"
      icon-left="check" />
    <div class="container">
      <div class="columns is-8 is-variable mt-6">
        <div class="column is-half">
          <div class="container mt-6">
            <b-image
              src="https://picsum.photos/1280/920"
              alt="A random image"
              ratio="6by4"
              :rounded="false"
            />
          </div>
        </div>
        <div class="column is-half">
          <intro class="mt-6" />
        </div>
      </div>
    </div>

    <div class="container">
      <presentation class="mt-6" />
    </div>

  </section>
</template>

<script>
import Intro from '~/components/Intro'
import Presentation from "@/components/Presentation";

export default {
  name: 'IndexPage',
  components: {
    Intro,
    Presentation
  },
}
</script>
