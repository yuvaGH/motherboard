<template>
 <header>
    <div class="logo">
        <img src="/img/Logo.png" alt="Logo">
    </div>
    <nav class="navigation">
      <ul>
        <li><a href="#">About</a></li>
        <li><a href="#">Faetures</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Testimonials</a></li>
        <li><a href="#">Help</a></li>
      </ul>
    </nav>
    <div class="authorization">
      <div class="sign-in"><button type="submit">Sing In</button></div>
      <div class="sign-up"><button type="submit">Sing Up</button></div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style>
body {
   font-family: Rubik;
   display: table;
   margin: 0 auto;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1146px;
  margin: 0 auto;
  padding: 0px 10px 0 10px;
}

ul>li {
 list-style: none;
}

.navigation ul {
  display: flex;
}

.navigation ul li a {
  color: #4F5665;
  font-size: 16px;
  text-decoration: none;
  list-style: none;
}


.navigation ul li:not(:last-child){
  margin-right: 40px;
}

.authorization {
  display: flex;
  align-items: center;
}

.sign-in {
  margin-right: 30px;

}

.sign-in button {
  text-decoration: none;
  color: unset;
  background-color: unset;
  border-color: unset;
  box-shadow: unset;
  border: none;
  font-size: 16px;
  color: #0B132A;
  font-weight: 700;
  line-height: 19px;
}

.sign-up button {
  padding: 13px 45px;
  border: 1px solid #F53855;
  border-radius: 50px;
  background-color: unset;
  color: #F53855;
  font-weight: 700;
}
</style>
