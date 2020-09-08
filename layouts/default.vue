<template>
  <div class="my-3">
    <!-- Header -->
    <div class="fixed-top">
      <div class="w-100 bg-dark text-white">
        <div class="container bg-dark">
          <div class="row py-2">
            <div class="col-md-12 pt-2"> 
              <span class="font-weight-bold" style="font-size: 24px;">
                <nuxt-link to="/" class="text-white text-decoration-none">UD</nuxt-link>
              </span>
              <div class="float-right pt-1 dropdown d-inline">
                jane.doe@udayhealth.org
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container mb-4" style="margin-top: 80px;">
      <div class="row">
        <div class="col-md-12">
          Uday APIs: 
          <nuxt-link to="/">Auth Features</nuxt-link> | 
          <nuxt-link to="ha-features">HA Features</nuxt-link> | 
          <nuxt-link to="admin-features-01">Admin Features 1</nuxt-link> | 
          <nuxt-link to="admin-features-02">Admin Features 2</nuxt-link> | 
          <nuxt-link to="admin-features-03">Admin Features 3</nuxt-link>
          <hr>
        </div>
      </div>
    </div>
    <nuxt />
  </div>
</template>

<style>

</style>
