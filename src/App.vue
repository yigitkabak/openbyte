<template>
  <div class="main-container">
    <div class="container">
      <div class="header">
        <h1>Yiğit</h1>
      </div>
      <div class="subheader">
        <BaseText />
      </div>
      <nav>
        <a href="https://github.com/yigitkabak" class="nav-link">github</a>
      </nav>
      <BaseFooter />
    </div>
  </div>
</template>

<style>
    body {
    background-color: #0a0a0a;
    background-image: 
      linear-gradient(to right, rgba(255, 255, 255, 0.05) 1px, transparent 1px),
      linear-gradient(to bottom, rgba(255, 255, 255, 0.05) 1px, transparent 1px);
    background-size: 20px 20px;
    margin: 0;
    min-height: 100vh;
    font-family: ui-monospace, Cascadia Code, Source Code Pro, monospace;
    -ms-overflow-style: none;
    scrollbar-width: none;
    overflow: hidden;
  }

  body::-webkit-scrollbar {
    display: none;
  }

  .main-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
  }

  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: calc(100vh - 3rem);
    padding: 2rem;
    color: #fff;
    gap: 3rem;
  }

  .header {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .logo {
    width: 64px;
    height: 64px;
    filter: brightness(0) invert(1);
  }

  h1 {
    font-size: 3.5rem;
    margin: 0;
    font-weight: 600;
    letter-spacing: -.03em;
  }

  .subheader {
    font-size: 1.15rem;
    opacity: .9;
    max-width: 32rem;
    text-align: center;
    line-height: 1.6;
  }
  
  .subheader a {
    color: #fff;
    text-decoration: none;
  }
  
  .subheader a:hover {
    opacity: 0.8;
  }

  .subheader p {
    margin: 0;
  }

  nav {
    display: flex;
    gap: 2.5rem;
  }

  .nav-link {
    color: #fff;
    text-decoration: none;
    font-size: 1.1rem;
    opacity: .8;
    transition: opacity .2s ease;
  }

  .nav-link:hover {
    opacity: 1;
    text-decoration: underline;
  }

  footer {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    text-align: center;
    font-size: .9rem;
    color: #767676;
    background-color: #111;
    padding: .75rem;
    border-top: 1px solid #222222;
  }

  footer p {
    margin: 0;
  }
</style>

<script>
  import BaseText from './components/Text.vue';
  import BaseFooter from './components/Footer.vue';
  
  export default {
  components: {
  BaseText,
  BaseFooter
  }
  }
</script>
