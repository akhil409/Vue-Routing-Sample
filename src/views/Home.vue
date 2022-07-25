<template>
  <div class="home">
           <v-container class="form">
              <v-row>
                  <v-col>
                       <v-form ref="signUpForm" v-model="formValidity" @submit.prevent="submitForm">
                            <h1 class="text center">Vuelidate Submit Form</h1>
                            <hr>
                            <v-text-field label="Title" v-model="title" :rules="titleRule" required ></v-text-field>

                            <v-text-field label="Firstname" v-model="firstName" ></v-text-field>

                            <v-text-field label="Lastname" v-model="lastName"></v-text-field>

                            <v-text-field label="Email" type="email" v-model="email" :rules="emailRule" required ></v-text-field>

                            <v-text-field label="Mobile Number" type="number" v-model="mobileNumber" ></v-text-field>

                            <v-text-field label="Organization" v-model="organization" ></v-text-field> 

                            <v-text-field label="Designation" v-model="designation" ></v-text-field>    

                            <v-textarea label="Address" v-model="address" ></v-textarea>

                            <v-text-field label="Password" v-model="password" ></v-text-field>

                            <v-text-field label="Confirm Password" v-model="confirmPassword" ></v-text-field>                      

                            <v-checkbox label="Agree to terms & conditions" v-model="agreeToTerms" :rules="agreeToTermsRules" required ></v-checkbox>

                            <v-btn class="mr-4" type="submit" color="primary" :disabled="!formValidity"  >Submit</v-btn>

                       </v-form>
                  </v-col>
              </v-row>
            </v-container>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {
   
  },
  data(){
    return{
      title:'',
    }
  }
}
</script>
