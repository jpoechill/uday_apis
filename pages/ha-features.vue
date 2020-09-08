<template>
  <div>
    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /registerpatient
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ stateID: '', name: '', age: '', ageType: '', phone: '', villOrCity: '', psId: '', districtId: '', stateId: '', sdwOf: '', occupationId: '', IND: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /getpatientlist
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{}"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {}
}
</script>

<style>
</style>
