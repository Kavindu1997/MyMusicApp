<template>
  <div class="container">
    <div class="row">
      <form class="form-horizontal">
        <fieldset>
          <legend>Welcome to Sarigama</legend>
          <app-search></app-search>
        </fieldset>
      </form>
    </div>

    <div class="row">
        <div class="col-md-12">
               <app-result></app-result>
        </div>
    </div>
  </div>
</template>

<script>
import SearchArea from './SearchArea.vue'
import ResultArea from './ResultArea.vue'

export default{
       components:{
           'app-result':ResultArea,
           'app-search':SearchArea
       }
}
</script>

<style>
</style>