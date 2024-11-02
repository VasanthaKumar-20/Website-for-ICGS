<template>
<div>  


  <div>

  <b-navbar toggleable="lg" type="dark" variant="info">
    
    <img src="https://seetharam.org.in/IMG-20231129-WA0003_1_-removebg-preview.png" width="180" height="150">
<b-nav fill>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>
<b-nav-item href="#"></b-nav-item>


    <b-navbar-brand href="#" align-brand="center">
      <h2><b>International Conference on Green Sustainable </b></h2>
        <h2><b>And Futuristic Technologies and Materials(ICGS FTM 2024)</b></h2>
</b-navbar-brand>
</b-nav>



    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
      
      </b-navbar-nav>

      
    </b-collapse>
  </b-navbar>
</div>





<div>
  <b-card>

  <div>
    <b-form-group
      id="fieldset-1"
      label="First_Name">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
  </div>

  <div>
    <b-form-group
      id="fieldset-1"
      label="Last_Name">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
  </div>

  <div>
    <p>DateOfBirth</p>
    <div>
    <b-form-datepicker v-model="value" :min="min" :max="max" locale="en"></b-form-datepicker>
  </div>
  </div>

  <div>
    <b-form-group
      id="fieldset-1"
      label="Country">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
  </div>

  <div>
    <b-form-group
      id="fieldset-1"
      label="State">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
  </div>

<div>
    <b-form-group
      id="fieldset-1"
      label="PinCode">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
</div>

<div>
    <b-form-group
      id="fieldset-1"
      label="Email">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
</div>

<div>
    <b-form-group
      id="fieldset-1"
      label="Mobile(Whatsapp)">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
</div>

<div>
    <b-form-group
      id="fieldset-1"
      label="Payment()">
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
</div>


  <div>
    <div class="mt-3">Upload you Screenshot {{ file1 ? file1.name : '' }}</div>

    <!-- Plain mode -->
    <b-form-file v-model="file2" class="mt-3" plain></b-form-file>
  </div>


  </b-card>
  </div>
</div>
</template>

<script>
  export default {
    data() {
      const now = new Date()
      const today = new Date(now.getFullYear(), now.getMonth(), now.getDate())
      // 15th two months prior
      const minDate = new Date(today)
      minDate.setMonth(minDate.getMonth() - 1000)
      minDate.setDate(15)
      // 15th in two months
      const maxDate = new Date(today)
      maxDate.setMonth(maxDate.getMonth() + 0)
      maxDate.setDate(15)

      return {
        value: '',
        min: minDate,
        max: maxDate
      }
    }
  }
</script>