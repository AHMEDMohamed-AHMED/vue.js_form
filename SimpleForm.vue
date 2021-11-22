<template>
<section>
  <div class="container">
    <form @submit.prevent="">
      <div class="form-group">
        <label for="fullName">fullName:</label>
        <input type="text" id="fullName" v-model="name">
      </div>

      <div class="form-group">
        <label for="email">email:</label>
        <input type="text" id="email" v-model="email">
      </div>

      <div class="form-group">
        <label for="massage">massege:</label>
        <input type="text" id="massage" v-model="massage" >
      </div>

      <button type="submit">Submit</button>
    </form>
  </div>
  <div>
    <p>RESULT</p>
    <p> name : {{name}}</p>
    <p>email : {{email}}</p>
    <p>massage:{{massage}}</p>
  </div>
</section>
</template>

<script>

export default {

data(){
  return{
    name:'',
    email:'',
    massage:''
  }
}

}

</script>


<style>
* {
  box-sizing: border-box;
  font-family: "Montserrat";
}
section {
  height: 100vh;
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.container {
  width: 90%;
  max-width: 500px;
  margin: 0 auto;
  padding: 20px;
  box-shadow: 0px 0px 20px #00000033;
  border-radius: 8px;
}
.form-group {
  margin-top: 20px;
  font-size: 20px;
  color: #9e9e9e;
}
.form-group input,
.form-group textarea {
  width: 100%;
  padding: 5px;
  font-size: 18px;
  border: 1px solid rgba(128, 128, 128, 0.199);
  margin-top: 5px;
}
button {
  width: 100%;
  border: none;
  padding: 20px;
  font-size: 24px;
  border-radius: 8px;
  cursor: pointer;
  margin-top: 10px;
}
p{
  text-align: left;
}

</style>