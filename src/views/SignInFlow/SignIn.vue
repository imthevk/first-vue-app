<template>
  <div class="container">
    <div class="request">
      Don't have a account?
      <router-link to="/request">Request an account</router-link>
    </div>
    <div class="login">
      <img src="@/assets/LogoV.png" alt />
      <h4>Sign into our webpage.</h4>
      <input type="email" placeholder="Enter your email" />
      <input type="password" placeholder="Enter your password" />
      <button>Sign In</button>
      <router-link to="/recover">Forgot your password</router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}
.login {
  width: 400px;
}
.request {
  position: absolute;
}
h4 {
  margin: 0;
  line-height: 34px;
  font-size: 24px;
  text-align: center;
}
input {
  background: rgba(255, 255, 255, 0.2);
  border: 1px solid rgba(255, 255, 255, 0.2);
  box-sizing: border-box;
  border-radius: 40px;

  height: 60px;
  width: 100%;

  font-size: 20px;
  color: #fff;
  padding-left: 20px;
  margin-top: 20px;

  &::placeholder {
    color: rgba(255, 255, 255, 0.3);
  }
}
button {
  background: #56ccf2;
  box-shadow: 0px, 0px, 20px, rgba(0, 0, 0, 0.2);
  border-radius: 40px;
  height: 60px;
  width: 100%;
  margin-top: 20px;
  margin-bottom: 40px;
  color: #fff;
  font-size: 20px;
}
a {
  margin-left: 20px;
  color: rgba(255, 255, 255, 0.3);
  line-height: 25px;
  text-align: center;
  text-decoration: none;
}
</style>