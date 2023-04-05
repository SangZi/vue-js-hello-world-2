<template>
  <h1>My Email is {{email}}</h1>
  <h1>My Mobole is {{mobile}}</h1>
  <h1>My Name is {{getName("Zi")}}</h1>
</template>

<script>
  export default {
    name: "MySecondCpmponent",
    data() {
      return {
        email: "zi.sang@testmail.de",
        mobile: "123456789",
        getName(name) {
          return name;
      }
      }
    }
  }

</script>