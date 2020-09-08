<template>
  <div>
    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requeststate
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ name: '', code: ''}]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestdistrict
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ code: '', name: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestps
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ name: '', code: '', state: '', district: '' }]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestoccupation
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[ 'occupation' ]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestappearance
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ objectid: '', name: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestgait
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ objectid: '', name: '' }]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestcategory
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ objectid: '', name: '' }]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestcomplaint
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ objectid: '', name: '', category: '' }]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestgeneralexam
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ objectid: '', name: '', organId: '', instructions: '' }]"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /requestspecificexam
        </div>
        <div class="col-md-6">
          <button>Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="[{ objectid: '', name: '', organId: '', complaint: '', instructions: '' }]"></textarea>
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
