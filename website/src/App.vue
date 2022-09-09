<template>
  <div class="bk-image">
    <html>
    <main>
      <header>
        <h1>Welcome to The Melbourne Butcher Shop </h1>
      </header>
      <p> Cart </p>
      <!-- <img
      src="https://images.unsplash.com/photo-1592686092916-672fa9e86866?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80"
      id="meatpic" alt="meat photo"> -->
      <p>
        Look at some of the Products down below now!
      </p>

    </main>

    <body>

      <div id="app">
        <component1></component1>

        <p> Email Name</p>
        <input v-model='email' placeholder="Please Enter Email" />
        <p>Email is: {{email}} </p>
        <p> Password </p>
        <input v-model='Password' type='text' placeholder="Enter Password" />
        <p>Password is: {{Password}}</p>

        <p> Location names: {{checkedNames}} </p>

        <input type='checkbox' id='Wantirna' value='Wantirna' v-model='checkedNames'>
        <label for="Wantirna">Wantirna</label>

        <input type='checkbox' id='Burwood' value='Burwood' v-model='checkedNames'>
        <label for="Burwood">Burwood</label>

        <input type='checkbox' id='CBD' value='CBD' v-model='checkedNames'>
        <label for="CBD">CBD</label>
      </div>

    </body>

    <p>
      Our Story.
      Our story begins all the way back in 1975 When Owners Margret and Greg opened the melbourne butcher shop It was
      a
      first of its kind with brand new cooling equipments.
    </p>
    <p>This also lead to a boost in customers and product longevity as store owners could make products last for
      longer
      and still taste the same.</p>

    </html>
  </div>
</template>

<script>

var component1 = {
  template: '<div> Hello Customer Thank you for ordering from Our Shop </div>'
}

export default {
  data() {
    return {
      email: '',
      Password: '',
      checkedNames: []
    }
  },
  components: {
    component1,
  }
}


</script>

<style>
header {
  font-family: 'Times New Roman', Times, serif;
  font-size: larger;
  color: #51f093;
  text-align: center;
  margin-top: 20px;
}



#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #06fa26;
  margin-top: 60px;
}

#app header {
  border: 1px solid black;
  box-shadow: 10px black;
}

p {
  font-size: large;
  color: rgb(63, 252, 104);
  margin-top: 10px;

}

* {
  margin: 0;
  padding: 0;
}

.bk-image {
  background-image: url('./steak.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
}
</style>



