<template>
  <div class="about">
    <h1 class="bold-black"> Započni s registracijom </h1>
    <div class="container">
      <div class="row">
        <div class="col-sm"></div>
        <div class="col-sm">
          <form @submit.prevent="registrirajKorisnika">
            <div class="form-group">
              <label for="ime">Unesite ime</label>
              <input v-model="ime" type="text" class="form-control" id="ime" placeholder="Unesite ime">
            </div>
            <div class="form-group">
              <label for="prezime">Unesite prezime</label>
              <input v-model="prezime" type="text" class="form-control" id="prezime" placeholder="Unesite prezime">
            </div>
            <div class="form-group">
              <label for="email">Email adresa</label>
              <input v-model="email" type="email" class="form-control" id="email" placeholder="Unesite svoju email adresu" />
            </div>
            <div class="form-group">
              <label for="lozinka">Lozinka</label>
              <input v-model="lozinka" type="password" class="form-control" id="lozinka" placeholder="Unesite svoju lozinku" />
            </div>
           
            <router-link to="/login-view">Registracija</router-link>
          </form>
        </div>
        <div class="col-sm"></div>
      </div>
    </div>
  </div>
</template>

<style>
body {
  background-color: #b4f1b4;
}

.bold-black {
  font-weight: bold;
  color: #000;
}

button[type="submit"] {
  background-color: #2ecc71;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>


<script>
export default {
  data() {
    return {
      ime: "",
      prezime: "",
      email: "",
      lozinka: ""
    };
  },
  methods: {
    registrirajKorisnika() {
      
    
}
  }
}
</script>
