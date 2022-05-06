<template>
  <div class="container has-text-justified">
    <h2 class="title is-2 mb-5">
      Bienvenue, je suis Maxime, étudiant en développement web.
    </h2>
    Étudiant <br class="mb-2" /> Mastère développement web & mobile <br class="mb-2" /> Ynov Bordeaux Campus

    <h5 class="subtitle is-5">Bonjour je suis maxime j'ai 23 ans et suis passionné par le monde informatique</h5>
    <div class="buttons">
      <b-button
        label="Linkedin"
        type="is-link is-light"
        icon-left="check" />
      <b-button
        label="Twitter"
        type="is-info is-light"
        icon-left="check" />
    </div>
<!--    <b-button
      label="Me contacter"
      type="is-primary"
      size="is-medium"
      icon-left="message-text"
      @click="isComponentModalActive = true" />

    <b-modal
      v-model="isComponentModalActive"
      has-modal-card
      trap-focus
      :destroy-on-hide="false"
      aria-role="dialog"
      aria-label="Example Modal"
      close-button-aria-label="Close"
      aria-modal>
      <template>-->
        <!-- Doit être mis dans un component externe -->
        <!--        <form action="">
                  <div class="modal-card" style="width: auto">
                    <header class="modal-card-head">
                      <p class="modal-card-title">Me contacter</p>
                    </header>
                    <section class="modal-card-body">
                      <h6 class="subtitle is-6 has-text-grey-light">contact@maximelarrieu.io</h6>
                      <b-field label="Email">
                        <b-input
                          type="email"
                          :value="email"
                          placeholder="Votre email"
                          required>
                        </b-input>
                      </b-field>

                      <b-field label="Message">
                        <b-input
                          type="textarea"
                          :value="message"
                          placeholder="Votre message"
                          required>
                        </b-input>
                      </b-field>

                    </section>
                    <footer class="modal-card-foot">
                      <b-button
                        label="Envoyer"
                        type="is-primary" />
                    </footer>
                  </div>
                </form>-->
        <!-- -->
<!--      </template>
    </b-modal>-->
  </div>
</template>

<script>
export default {
  name: 'WebsiteIntro',
}
</script>
