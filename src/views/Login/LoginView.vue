<template>
  <section class="form-area">
    <div class="form-container">
      <h1>Login</h1>
      <form>
        <div>
          <label for="email">Email Address</label>
          <input type="email" name="email" id="email" />
        </div>
        <div>
          <label for="password">Password</label>
          <input type="password" name="password" id="password" />
        </div>
        <div>
          <input type="checkbox" name="remember" id="remember" />
          <label for="remember">Remember Password</label>
        </div>

        <router-link to="/home">
          <button class="btn">Login</button></router-link
        >
        <p class="no-account">
          Don’t have an account?
          <router-link to="/short-profile" class="sign-up">
            Sign up
          </router-link>
        </p>

        <span>or</span>
        <router-link to="/home">
          <button class="btn-alt">
            <img src="@/assets/icons/google-icon.png" class="google-icon" />
            <span> Authorize with Google </span>
          </button></router-link
        >
      </form>
    </div>
  </section>
  <welcome-image />
</template>

<script>
import WelcomeImage from "@/components/WelcomeImage.vue";
export default {
  name: "LoginView",
  components: {
    WelcomeImage,
  },
};
</script>

<style>
.form-area {
  width: 50%;
  display: grid;
  place-content: center;
}
.form-container {
  min-width: 500px;
}

.form-container h1 {
  font-size: 48px;
  margin-bottom: 48px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 24px;
}

label {
  color: #121212;
  display: block;
  margin-bottom: 16px;
  font-size: 20px;
  font-weight: 400;
}

label[for="remember"] {
  color: #121212;
  display: inline-block;
  margin-left: 16px;
}

input[type="checkbox"] {
  height: 14px;
  display: inline-block;
  background-color: var(--purple);
  width: 14px;
}

button {
  padding: 20px 10px;
  border: none;
  border-radius: 8px;
  font-size: 20px;
  width: 100%;
}

.btn {
  background: var(--purple);
  color: white;
}

.btn-alt {
  gap: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1px solid var(--black);
  color: var(--black);
  background: var(--white);
}

.sign-up {
  font-weight: bold;
  color: var(--purple);
}

.no-account {
  font-size: 20px;
}

.no-account a {
  color: var(--purple);
}

.form-area span {
  text-align: center;
  font-size: 20px;
}
</style>







