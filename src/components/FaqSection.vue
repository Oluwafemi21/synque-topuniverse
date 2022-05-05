<template>
  <section class="middle">
    <div class="heading">
      <h2>FAQs</h2>
      <p>How can we help you?</p>
    </div>
    <form>
      <input
        type="text"
        class="form-input"
        placeholder="Please enter your question"
      />
      <input class="form-btn" type="submit" value="Send" />
    </form>
    <!-- <section class="questions">
      <article>
        <div class="question-header">
          <h4>
            <i class="fa-solid fa-arrow-right"></i>
            How many pictures am I allowed to upload?
          </h4>
          <p>
            There is no limit to the number of images you can upload on your
            account, as number depends on the owner of the account.
          </p>
        </div>
      </article>

      <div class="confirmation">
        <p>Was this article helpful?</p>
        <div class="confirmation-container">
          <button>Yes</button>
          <button>No</button>
        </div>
        <button>Help Center</button>
      </div>
    </section> -->
  </section>
</template>

<script>
export default {
  name: "FaqSection",
};
</script>

<style scoped>
.middle {
  flex: 1;
  height: 100%;
  padding: 4rem 8rem 4rem 2.5rem;
  background-color: #fcfcfc;
}

.heading {
}

.heading h2 {
  font-size: 3.2rem;
}

.heading h2 i {
  margin-right: 1.2rem;
}

.heading p {
  font-size: 1.8rem;
  color: var(--black);
  opacity: 0.7;
  font-weight: 400;
  margin-block: 2.2rem 1.4rem;
}

form {
  background-color: #eeeeee;
  position: relative;
  margin-bottom: 2.5rem;
  margin-right: 1.7rem;
  border-radius: 8px;
  display: flex;
  height: 58px;
}

form .form-input {
  background-color: transparent;
  width: 100%;
  font-size: 1.6rem;
  padding: 29px 40px;
  border-radius: 8px;
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
  border: none;
  outline: none;
}

form .form-input::placeholder {
  color: #525252;
  opacity: 0.5;
  font-weight: 400;
  font-size: 1.4rem;
}

form .form-btn {
  background-color: var(--purple);
  color: white;
  font-size: 1.6rem;
  border-radius: 8px;
  height: 100%;
  padding-inline: 7.5rem;
  border: none;
  cursor: pointer;
}
</style>