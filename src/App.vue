<template>
  <div class="container">
    <div class="wrapper">
      <div class="wrapper__logo flex-center">
        <img src="../assets/imgs/logo.png" alt="" />
        <p>Chatvia</p>
      </div>
      <!--wrapper__logo-->
      <div class="wrapper__header flex-center">
        <span>Sign in</span>
        <p>Sign in to continue to VueChat.</p>
      </div>
      <!--wrapper__header-->
      <div class="login__form">
        <form>
          <div class="form__username">
            <label>Username</label>
            <input
              class="username-input"
              type="text"
              name="username"
              placeholder="Enter Username"
              id="username"
            />
          </div>
          <!--form__username-->

          <div class="form__password">
            <label>Password</label>
            <input
              class="password-input"
              type="password"
              name="password"
              placeholder="Enter password"
              id="password"
            />
          </div>
          <!--form__password-->

          <div class="form__rememberme">
            <input type="checkbox" id="rem" name="rememberMe" value="rem" />
            <label>RememberMe</label>
          </div>
          <!--form__rememberme-->

          <div class="form__signin">Sign in</div>
          <!--form__signin-btn-->
        </form>
        <!--form-->
      </div>
      <!--login__form-->
      <div class="login__footer">
        <p>Don't have an account ?</p>
        <a href="#">Signup now </a>
      </div>
      <!--login__footer-->
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({})
export default class App extends Vue {}
</script>

<style lang="scss">
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  min-width: 100vw;
  background-color: $primary-bg-color;
}

.wrapper__logo {
  font-weight: 700;
  margin-bottom: 35px;
  font-size: 22px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  img {
    width: 25px;
    margin-right: 5px;
  }
}

.wrapper__header {
  span {
    font-size: 20px;
    color: $primary-p-dark-color;
  }

  p {
    color: $primary-p-light-color;
  }
}
.login__form {
  background-color: #fff;
  padding: 45px;
  border-radius: 10px;
  margin: 20px 0 50px 0;
  width: 500px;

  .username-input,
  .password-input {
    width: 100%;
    padding: 18px 20px;
    margin: 4px 0 25px 0;
    border-radius: 10px;
    border: 2px solid #e6ebf5;
    background-color: #f9fafd;
  }

  .form__rememberme {
    input {
      margin: 15px 5px 15px 0;
    }
  }

  .form__signin {
    display: flex;
    border-radius: 4px;
    width: 100%;
    height: 45px;
    font-size: 13px;
    font-weight: 600;
    text-transform: uppercase;
    padding: 0 30px;
    letter-spacing: 1px;
    align-items: center;
    justify-content: center;
    text-align: center;
    border: none;
    background-color: $primary-color;
    color: #fff;
    cursor: pointer;
  }
}
</style>
