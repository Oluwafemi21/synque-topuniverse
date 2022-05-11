<template>
  <main>
    <div class="navbar">
      <a href="#notification">Notifications</a>
      <a href="#newfeatures">New Features</a>
      <a href="#help">Help</a>
      <a href="#search">Search</a>
      <a href="#faq">FAQs</a>
    </div>
    <div class="heading">
      <div class="head flex-space-btw w-95">
        <h1>Settings</h1>
        <h3>Hello Morenike,</h3>
        <div class="toggle-wrap">
          <p>
            Synq.ue is the idael platform for content creators and entrepreneurs
            to display their amazing contents and products<br />
            Would you like to switch on my Synq.ue page?
          </p>
          <label class="switch">
            <input type="checkbox" />
            <span class="slider round"></span>
          </label>
        </div>
        <h3>Profile Settings</h3>
      </div>
    </div>
    <div class="form">
      <div class="avatar">
        <!-- <img src="@/assets/images/profile-img.png" alt="Avatar" /> -->
      </div>

      <div class="colums">
        <div class="item">
          <label for="name">Full Name</label>
          <input
            id="name"
            type="text"
            name="name"
            placeholder="Enter full name"
          />
        </div>
        <div class="item">
          <label for="username">Username</label>
          <input
            id="username"
            type="text"
            name="username"
            placeholder="Enter username"
          />
        </div>
        <div class="item">
          <label for="email-address">Email Address</label>
          <input
            id="email-address"
            type="text"
            name="email-address"
            placeholder=" Enter email-address"
          />
        </div>
        <div class="item">
          <label for="specification">Specifications</label>
          <input
            id="specification"
            type="text"
            name="specification"
            placeholder="Select Applicable Area (3 Max)"
          />
        </div>
        <div class="profile-btn-align">
          <button class="profile-btn1">
            Tech<img src="assets/Cancel-icon.png" />
          </button>
          <button class="profile-btn2">
            Entrepreneur<img src="assets/Cancel-icon.png" />
          </button>
        </div>
      </div>
    </div>

    <button class="save-d-btn">Save Details</button>

    <div class="box">
      <p id="text-1">Change Password</p>
      <div class="align-btn">
        <p id="text-2">Change your current password to a new one</p>
        <button class="click-btn">Change Password</button>
      </div>
    </div>
    <div class="box">
      <p id="text-1">Manage Account</p>
      <div class="align-btn">
        <p id="text-2">
          You can add switch to another account you registered on Synq.ue and
          manage them
        </p>
        <button class="click-btn">Manage Account</button>
      </div>
    </div>
    <div class="box">
      <p id="text-1">Notifications</p>
      <div class="align-btn">
        <p id="text-2">Receive notifications from us via your emails</p>
        <label class="switch">
          <input type="checkbox" />
          <span class="slider round"></span>
        </label>
      </div>
    </div>

    <h3>Delete Account</h3>
    <div class="box">
      <div class="align-btn1">
        <p id="text-2">
          Your account will no longer be available, and your data will
          permanently be deleted
        </p>
        <button class="del-btn">Delete Account</button>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "SettingsView",
};
</script>

<style scoped>
main {
  flex: 1;
  height: 100%;
  padding: 4rem 8rem 4rem 2.5rem;
  background-color: #fcfcfc;
  margin-left: 331px;
  overflow-x: hidden;
}

.main-content .heading {
  padding: 8rem 3rem 1.2rem;
}
.main-content .heading h1 {
  margin-bottom: 2rem;
  font-size: 30px;
  font-family: Metropolis;
  font-weight: 700;
}
.main-content .heading h3 {
  font-size: 24px;
  font-family: Metropolis;
  font-weight: 500;
  margin-bottom: 0.9rem;
}
.toggle-wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 910px;
  height: 80px;
  /*box-shadow: 0 3px 10px rgb(0 0 0 / 0.2);*/
}
.main-content .heading p {
  line-height: 1.8;
  margin-bottom: 1rem;
  font-size: 15px;
  font-family: Metropolis;
  font-weight: 300;
}

.switch {
  margin-left: px;
  position: relative;
  display: inline-block;
  width: 56px;
  height: 28px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: #d0b5e0;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 20px;
  width: 20px;
  left: 4px;
  bottom: 4px;
  background: #543864;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background: #d0b5e0;
}

input:focus + .slider {
  box-shadow: 0 0 1px #543864;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

.main-content .form {
  padding: 40px;
  width: 870px;
  height: 340px;
  background: #ffffff;
  margin-bottom: 30px;
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.2);
}

.avatar {
  vertical-align: middle;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin-bottom: 80px;
}

.colums {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  flex-wrap: wrap;
}
.colums div {
  width: 48%;
  margin-bottom: 10px;
}

input[type="text"] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  background: #eeeeee;
  border: none;
  border-radius: 4px;
  box-sizing: border-box;
  font-size: 14px;
  font-family: Metropolis;
  font-weight: 500;
}

.item label {
  font-size: 16px;
  font-family: Metropolis;
  font-weight: 500;
}

.profile-btn-align {
  display: flex;
  margin-left: 452px;
}

.profile-btn1 {
  display: flex;
  margin-right: 16px;
  width: 110px;
  align-items: center;
  justify-content: center;
  background: #ffbd69;
  color: #ffffff;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-family: Metropolis;
  font-size: 16px;
  font-weight: 500;
}
.profile-btn1 img {
  padding: 8px;
  align-items: center;
}

.profile-btn2 {
  display: flex;
  width: 190px;
  align-items: center;
  justify-content: center;
  color: #ffffff;
  background: #ffbd69;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-family: Metropolis;
  font-size: 16px;
  font-weight: 500;
}
.profile-btn2 img {
  padding: 8px;
  align-items: center;
}

.save-d-btn {
  width: 150px;
  font-size: 16px;
  font-family: Metropolis;
  font-weight: 500;
  padding: 12px 10px;
  background-color: #543864;
  color: #ffffff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  margin-bottom: 60px;
}
.main-content .box {
  padding: 30px;
  width: 870px;
  height: 80px;
  background: #ffffff;
  margin-bottom: 30px;
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.2);
}

.box .align-btn {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: -10px;
}

.click-btn {
  margin-top: -10px;
  width: 190px;
  font-size: 16px;
  padding: 12px 10px;
  background: #ffffff;
  color: #543864;
  border: 1px solid #543864;
  border-radius: 5px;
  cursor: pointer;
}

.box #text-1 {
  font-size: 20px;
  font-family: Metropolis;
  font-weight: 500;
}
.box #text-2 {
  font-size: 16px;
  font-family: Metropolis;
  font-weight: 400;
}

.box .align-btn1 {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 30px;
}

.del-btn {
  margin-top: -10px;
  width: 190px;
  font-size: 16px;
  padding: 12px 10px;
  background: #f22929;
  color: #ffffff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>