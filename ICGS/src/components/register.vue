<template>
  <div>
    <div id="bg"></div>

<div class= "col-md-6 mx-auto p-0">

  <b-card style="max-width: 30rem;"
class = "mr-center"
img-src="https://d35fo82fjcw0y8.cloudfront.net/2018/06/01005211/Bookmyshow-logo.png"
>
 <b-form>

   <b-form-group label="Email or Mobile">
     <b-form-input v-model="name"  required placeholder = "Mail/Mobile">
     </b-form-input>
   </b-form-group>

 <b-form-group label="User_name">
     <b-form-input v-model="issues" required placeholder = "User_name">
     </b-form-input>
   </b-form-group>

    <b-form-group label="Password">
      <b-form-input v-model="email" required placeholder = "#8_Characters">
      </b-form-input>
   </b-form-group>

    <b-form-group label="Confirm Password">
      <b-form-input v-model="email" required placeholder = "#8_Characters">
      </b-form-input>
   </b-form-group>

   <md-button v-on:click="success()" class="md-raised md-accent">Submit</md-button>
<br>


</b-form>
</b-card>


</div>

</div>
</template>

import success from '@/components/success'
<script>
export default {
    data() {
            return {
                
            }
        },
    methods: {
        success() {
            this.$router.push('/login1')
        }
    }
}
</script>

