<template>
  <div>
    <Navbar/>
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <div class="col-md-3">
            <Sliderbar/>
          </div>
          <div class="col-md-9">
            <router-view></router-view>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
  import Navbar from '@/components/Navbar';
  import Sliderbar from '@/components/Sliderbar'
  export default {
    components: {
      Navbar,
      Sliderbar
    }
  }
</script>

<style>

</style>
