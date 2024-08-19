<template>
  <div id="app">
    <header>
      <nav>
        <a href="#">Gmail</a>
        <a href="#">이미지</a>
        <button class="apps-button">
          <i class="material-icons">apps</i>
        </button>
        <button class="signin-button">로그인</button>
      </nav>
    </header>
    <main>
      <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="Google" class="logo">
      <div class="search-container">
        <input type="text" class="search-input">
        <div class="search-buttons">
          <button>Google 검색</button>
          <button>I'm Feeling Lucky</button>
        </div>
      </div>
    </main>
    <footer>
      <div class="footer-left">
        <a href="#">광고</a>
        <a href="#">비즈니스</a>
        <a href="#">Google 정보</a>
        <a href="#">검색의 원리</a>
      </div>
      <div class="footer-right">
        <a href="#">개인정보처리방침</a>
        <a href="#">약관</a>
        <a href="#">설정</a>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
#app {
  font-family: Arial, sans-serif;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  padding: 20px;
  text-align: right;
}

nav a, nav button {
  margin-left: 15px;
  text-decoration: none;
  color: #000;
}

.apps-button, .signin-button {
  background: none;
  border: none;
  cursor: pointer;
}

.signin-button {
  background-color: #4285f4;
  color: white;
  padding: 9px 23px;
  border-radius: 3px;
}

main {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  margin-bottom: 20px;
}

.search-container {
  text-align: center;
}

.search-input {
  width: 500px;
  padding: 10px;
  border: 1px solid #dfe1e5;
  border-radius: 24px;
  font-size: 16px;
}

.search-buttons {
  margin-top: 20px;
}

.search-buttons button {
  margin: 0 5px;
  padding: 10px 16px;
  background-color: #f8f9fa;
  border: 1px solid #f8f9fa;
  border-radius: 4px;
  color: #3c4043;
  cursor: pointer;
}

footer {
  background-color: #f2f2f2;
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
}

footer a {
  color: #70757a;
  text-decoration: none;
  margin-right: 15px;
}
</style>