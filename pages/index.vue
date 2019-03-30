<template>
  <div>
    <header>
      <Navbar />
      <div class="space-navbar"></div>
    </header>
    <section class="container ">
      <div class="text-center">
        <logo />
        <h1 class="title">
          fahmadrifki-dev-nuxt
        </h1>
        <h2 class="subtitle">
          fahmadrifki.github.io developer tools
        </h2>
        
      </div>
    </section>
    <section class="container ">
      <div class="text-center">
        <logo />
        <h1 class="title">
          fahmadrifki-dev-nuxt
        </h1>
        <h2 class="subtitle">
          fahmadrifki.github.io developer tools
        </h2>
        
      </div>
    </section>
    <section class="container ">
      <div class="text-center">
        <logo />
        <h1 class="title">
          fahmadrifki-dev-nuxt
        </h1>
        <h2 class="subtitle">
          fahmadrifki.github.io developer tools
        </h2>
        
      </div>
    </section>
    <section class="container ">
      <div class="text-center">
        <logo />
        <h1 class="title">
          fahmadrifki-dev-nuxt
        </h1>
        <h2 class="subtitle">
          fahmadrifki.github.io developer tools
        </h2>
        
      </div>
    </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Navbar from '~/components/Navbar.vue'

export default {
  components: {
    Logo,
    Navbar
  }
}
</script>

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}  */

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.space-navbar{
  padding-top: 6.5rem;
}
</style>
