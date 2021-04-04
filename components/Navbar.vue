<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <nuxt-link class="navbar-brand" to="/">Firengii</nuxt-link>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <nuxt-link class="nav-link" to="/products">Products <span class="sr-only">(current)</span></nuxt-link>
      </li>
      <li class="nav-item">
        <nuxt-link class="nav-link" to="/products/id">My Items</nuxt-link>
      </li>
    
    </ul>

  </div>
</nav>
</template>

<script>
export default {

}
</script>

<style>

</style>