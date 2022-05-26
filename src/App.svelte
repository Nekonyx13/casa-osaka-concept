<script>
    export let name;
</script>

<main>
    <div class="content">
        <header>
            <div class="logo-container">
                <img src="/assets/logo.png" class="logo-img">
                <div class="logo-with-nav">
                    <img src="/assets/logo_text.svg" class="logo-text">

                    <nav>
                        <ul class="nav-list">
                            <li class="nav-item">
                                <a href="/" class="nav-link">Home</a>
                            </li>
                            <li class="nav-item">
                                <a href="/about" class="nav-link">About</a>
                            </li>
                            <li class="nav-item">
                                <a href="/contact" class="nav-link">Contact</a>
                            </li>
                            <li class="nav-item">
                                <a href="/login" class="nav-link">Login</a>
                            </li>
                            <li class="nav-item">
                                <a href="/login" class="nav-link">Login</a>
                            </li>
                            <li class="nav-item">
                                <a href="/login" class="nav-link">Login</a>
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </header>
    </div>
</main>

<style lang="scss">
  main {
    width: 100vw;
    height: 100vh;
    background-size: cover;
    background: hsla(0, 0%, 0%, 0.45) url("/assets/background.jpg") no-repeat top;
    background-size: cover;
    background-blend-mode: darken;
  }

  .content {
    margin: auto;
    height: 100vh;

    width: 55vw;
    min-width: 768px;
    background: hsla(0, 39%, 37%, 0.52);

    @media (max-width: 768px) {
      width: 100vw;
      min-width: 100vw;
    }
  }

  header {
    display: flex;
    align-items: center;
    background: hsla(196, 40%, 42%, 0.52);
  }

  .logo-container {
    display: flex;
    background: hsla(75, 40%, 42%, 0.52);
    padding: 2em;
    width: 100%;

    .logo-img {
      object-fit: cover;
      height: 7em;
    }

    .logo-text {
      background: hsla(75, 40%, 42%, 0.52);
      flex: 1;
      margin-right: auto;
    }

    .logo-with-nav {
      display: flex;
      flex-direction: column;
      margin-left: 1em;

      width: 100%;
    }
  }

  nav {
    background-color: hsla(264, 59%, 21%, 0.6);
    border-radius: 0.5em;
    color: white;

    max-width: 40em;

    position: relative;

    $margin: 1.5em;
    top: $margin;
    margin-top: -$margin * 0.5;
  }

  .nav-list {
    display: flex;
    align-items: center;
    justify-content: space-around;

    padding: 0;

    .nav-item {
      display: flex;
      align-items: center;
      justify-content: center;

      color: hsla(0, 0%, 100%, 0.8);
      font-size: 1em;

      a {
        color: hsla(0, 0%, 100%, 0.8);
        text-decoration: none;

        &:hover {
          color: hsl(237, 42%, 61%);
        }
      }
    }
  }
</style>