<template>
  <nav class="navbar navbar-expand-lg fixed-top fa-navbar" v-bind:class="{ 'animation': fixedOnScroll }">
    <div class="container">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item active">
            <a class="nav-link" href="#">Specialties</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Profile</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Portfolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style lang="sass" scoped>

$green: #41B883

.fa-navbar
  background-color: rgba(0,0,0,0)
  padding: 2rem 0


.fa-navbar,
.animation
  transition: 0.5s
  -webkit-transition: 0.5s


.fa-navbar.animation
  background-color: #fff
  border-bottom: 1px solid #ececec
  box-shadow: 0 3px 8px rgba(0,0,0,.1)
  padding: 0.1rem
  margin: 0 auto

.nav-link
  color: #333
  padding: .5rem .95rem

  &:hover
    color: $green
    border-bottom: 3px solid $green

</style>

<script>
  export default {
    name: 'MainNav',
    data: function () {
      return {
        fixedOnScroll: false
      }
    },
    methods: {
      handleScroll () {
        if (window.scrollY >= 100) {
          this.fixedOnScroll = true
        } else {
          this.fixedOnScroll = false
        }
      }
    },
    created () {
      if (process.browser) {
        window.addEventListener('scroll', this.handleScroll)
      }
    },
    beforeUpdate () {
      if (process.browser) {
        window.addEventListener('scroll', this.handleScroll)
      }
    }
  }
</script>