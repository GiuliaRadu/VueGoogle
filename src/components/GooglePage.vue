<template>
  <div class="entire">
    <b-nav>
      <b-nav-item disabled class="text-link">Gmail</b-nav-item>
      <b-nav-item disabled class="text-link">Images</b-nav-item>
      <b-nav-item disabled class="icon-link">
        <img src="../assets/g-menu.png" />
      </b-nav-item>
      <b-nav-item disabled class="icon-link">
        <img src="../assets/account.png" />
      </b-nav-item>
    </b-nav>
    <section class="form-section">
      <div class="logo">
        <img src="../assets/google.png" />
      </div>
      <b-form class="search">
        <div class="input-container">
          <img src="../assets/search.svg" class="search-icon" />
          <b-form-input
            id="inline-form-input-name"
            class="search-input"
          ></b-form-input>
          <img src="../assets/vs.png" class="vs-icon" />
        </div>
      </b-form>
      <div class="buttons">
        <button class="s-button">Google Search</button>
        <button class="s-button">I'm feeling Lucky</button>
      </div>
      <div class="lang">
        Google offered in:
        <a href="#">Romana</a>
        <a href="#">Magyar</a>
        <a href="#">Deutsch</a>
      </div>
    </section>
    <div class="footer">
      <h4>Romania</h4>
      <div class="links">
        <div class="link-1">
          <a href="#">Advertising</a>
          <a href="#">Business</a>
          <a href="#">About</a>
          <a href="#">How Search works</a>
        </div>
        <div class="link-2">
          <a href="#">Privacy</a>
          <a href="#">Terms</a>
          <a href="#">Settings</a>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: "GooglePage",
  data() {
    return {
      mainProps: {
        blank: true,
        blankColor: "#777",
        width: 75,
        height: 75,
        class: "m1",
      },
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.search-icon {
  width: 20px;
  opacity: 0.4;
  position: absolute;
  top: 10px;
  left: 14px;
}

.vs-icon {
  width: 14px;
  position: absolute;
  top: 10px;
  right: 24px;
}

.text-link:first-child {
  margin-right: 15px;
}

.lang {
	margin-top: 30px;
	text-align: center;
	font-size: 13px;
	color: #111;
}
.lang a {
	margin-left: 5px;
	color: #1a0dab;
}
.lang a:hover {
	text-decoration: underline;
}
.nav {
  padding: 6px;
  align-items: center;
  justify-content: flex-end;
}

.nav-item:nth-child(2) {
  padding-right: 15px;
}

.nav-item {
  height: 48px;
}

.nav-item a {
  padding: 0;
  height: 100%;
  font-size: 14px;
  color: black;
  display: flex;
  align-items: center;
}

.nav-item img {
  height: 35px;
  width: 35px;
}

.icon-link:last-child {
  margin-left: 10px;
}

.search {
  width: 580px;
  padding: 20px;
}

.search-input {
  border-radius: 25px;
  padding-left: 45px;
}

.form-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.buttons {
  outline: none;
  cursor: pointer;
}

.s-button {
  background-color: #f8f9fa;
  border: 1px solid #f8f9fa;
  border-radius: 4px;
  color: #3c4043;
  font-family: arial, sans-serif;
  font-size: 14px;
  margin: 11px 4px;
  padding: 0 18px;
  line-height: 27px;
  height: 36px;
  min-width: 54px;
  text-align: center;
}

.s-button:hover {
  text-decoration: underline;
  box-shadow: 0 1px 1px rgb(0 0 0 / 10%);
  background-color: #f8f9fa;
  border: 1px solid #dadce0;
  color: #202124;
}

.entire {
  height: 100%;
}

.logo {
  padding-top: 100px;
  margin-bottom: 15px;
}

.input-container {
  position: relative;
}

.footer {
  background: #f2f2f2;
  position: absolute;
  bottom: 0;
  width: 100%;
  text-align: initial;
}
.footer h4 {
  color: rgba(0, 0, 0, 0.54);
  font-size: 15px;
  line-height: 39.5px;
  font-weight: 400;
  padding-left: 29px;
  border: 1px solid #eee;
}
.footer a {
  color: #5f6368;
  display: inline-block;
  padding: 12px 11.3px;
  font-size: 14px;
}
.footer a:hover {
  text-decoration: underline;
}
.links {
  border-top: 1px solid #ddd;
  display: flex;
}
.link-1 {
  padding-left: 18.7px;
  flex: 1;
}
.link-2 {
  padding-right: 18.7px;
}
</style>
