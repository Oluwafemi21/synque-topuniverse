<template>
  <section class="form-area">
    <div class="form-container">
      <div class="welcome">
        <h1>Welcome to Synque</h1>
        <div class="para">
          <p>
            Here you can create your personalized mini website <br />
            for lorem ipseum dolor ite
          </p>

          <p>
            Already have an account? <router-link to="/">Sign In</router-link>
          </p>
        </div>
      </div>

      <form>
        <div>
          <label for="username">Username</label>
          <input type="text" name="username" id="username" />
        </div>
        <div>
          <label for="email">Email</label>
          <input type="email" name="email" id="email" />
        </div>
        <div>
          <label for="password">Password</label>
          <input type="password" name="password" id="password" />
        </div>
        <button type="submit" class="btn">Submit</button>
        <div class="signUpAlt">
          <span>or sign up with</span>
          <div class="signUpImg">
            <a href="#">
              <img src="@/assets/icons/google-icon.png" />
            </a>
            <a href="#">
              <img
                src="@/assets/icons/facebook-logo-2019.png"
                class="facebook"
              />
            </a>
          </div>
        </div>
      </form>
    </div>
  </section>
  <welcome-image />
</template>

<script>
import WelcomeImage from "@/components/WelcomeImage.vue";
export default {
  name: "WelcomeView",
  components: {
    WelcomeImage,
  },
};
</script>

