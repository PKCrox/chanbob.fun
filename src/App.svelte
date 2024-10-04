<script>
  let backgroundColor = '#f4f4f4';

  function changeBackgroundColor() {
    backgroundColor = '#' + Math.floor(Math.random()*16777215).toString(16);
  }
</script>

<main style="background-color: {backgroundColor}">
  <header>
    <h1>Chanbob's Fun Space</h1>
  </header>
  <div class="content">
    <p>안녕하세요! Chanbob의 개인 웹사이트에 오신 것을 환영합니다.</p>
    <button on:click={changeBackgroundColor}>배경색 변경</button>
  </div>
  <footer>
    <p>&copy; 2024 Chanbob. All rights reserved.</p>
  </footer>
</main>

<style>
  main {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 20px;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }

  header {
    background-color: #35424a;
    color: white;
    text-align: center;
    padding: 1rem;
    border-radius: 5px;
  }

  .content {
    flex-grow: 1;
    max-width: 800px;
    margin: 20px auto;
    padding: 20px;
    background-color: white;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
  }

  button {
    background-color: #35424a;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 16px;
  }

  button:hover {
    background-color: #2c3e50;
  }

  footer {
    text-align: center;
    margin-top: 20px;
    color: #777;
  }
</style>