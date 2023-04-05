<template>
  <h1>My Email is {{getContactInfo().email}}</h1>
  <h1>My Mobile is {{getContactInfo().mobile}}</h1>
  <h1>My Name is {{getName("Zi")}}</h1>
</template>

<script>
  export default {
    name: "MySecondComponent",
    data() {
      return {
        email: "zi.sang@testmail.de",
        mobile: "123456789",

      }
    },
    methods: {
      getName(name) {
        return name;
      },
      getContactInfo() {
        return {
          email: this.email, //with "this.email", here it gets the value from data()
          mobile: this.mobile
        }
      }
    }
  }
</script>