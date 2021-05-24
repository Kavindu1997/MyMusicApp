<template>
      <div class="form-groups">
            <label for="dynamicSearch" class="col-sm-2 col-form-label">Search Music</label>
            <div class="col-sm-10">
              <input type="text" class="form-control" id="dynamicSearch" placeholder="Type here..." @input="typing" />
            </div>
      </div>
</template>

<script>
import axios from 'axios'
export default{
    methods:{
        typing(event){
            var query=event.target.value;
            //console.log(query);
            // axios.get("https://api.spotify.com/v1/search?q="+query+"&type=track").then(response=>{
            //     console.log(response.data)
            // }).catch(e=>{
            //     this.error.push(e)
            // })

        }
    }

}

</script>

<style>

</style>
