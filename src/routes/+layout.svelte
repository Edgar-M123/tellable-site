<script lang='ts'>
    let {children} = $props()
    import LogoButton from "$lib/components/LogoButton.svelte";

    let supportEmail = "contact@tellableapp.com"


</script>

<main class="container">

    <div class="content">
        <!-- Logo and title -->

        <LogoButton />
    
        <nav class="buttons">
            <a class="nav-button primary" href="/download" target="_blank">Download&nbsp;<span class="external-icon"></span></a>
            <!-- <a class="nav-button" href="/subscribe">Subscribe</a>
            <a class="nav-button" href="/leaderboard">Leaderboard</a>
            <a class="nav-button" href="/blog">Blog</a> -->
            <a class="nav-button" href="/contact">Contact</a>
        </nav>

        <!-- <LoginSignup/> -->
        
    </div>

</main>

{@render children()}


<footer>

    <div class="section-items" style="justify-content: space-evenly">

      <div class="footer-text">
        <p style="color: grey">Property of Edgar Martinez Chavez</p>
        <p style="color: grey">Contact me at <a style="color: #0077b6" href="mailto:{supportEmail}">{supportEmail}</a></p>
      </div>

      <div class="footer-links">
        <nav>
          <h3>Legal</h3>
          <ul style="list-style-type: none; padding: 0px;">
            <li><a href="/privacy">Privacy Policy</a></li>
            <li><a href="/csae">CSAE Standards</a></li>
          </ul>
        </nav>
      </div>

    </div>

  </footer>


<style>

    :root {

        --surface: hsl(225, 76%, 3%);
        --surfaceHover: hsl(225, 76%, 16%);
        --onSurface: #ffffff;
        --onSurfaceHover: #c1c6d7;
        --surfaceOutline: #8b90a0;
        --primary: hsl(225, 73%, 57%);
        --primaryHover: hsl(225, 73%, 50%);
        --onPrimary: #ffffff;
        --accent: hsl(10, 100%, 70%);
        --accentHover: hsl(10, 100%, 62%);
        --surfaceContainerMed: hsl(220, 33%, 21%);
        --surfaceContainerMedHover: hsl(220, 33%, 14%);
        --error: #93000a;
        --onError: #ffdad6;

        --content-width: 1200px;

        line-height: 1.5;
        font-weight: 400;
        font-family: "Merriweather", serif, system-ui, Avenir, Helvetica, Arial, sans-serif;
        font-synthesis: none;
        max-width: 100vw;

        margin: 0;
        overflow-x: hidden;

        color-scheme: light dark;
        color: var(--onSurface);
        background-color: var(--surface);

        text-rendering: optimizeLegibility;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;

        -webkit-overflow-scrolling: touch;
        overscroll-behavior-y: auto;
    }

    :global body {
        margin: 0;
        max-width: 100vw;
        overflow-x: hidden;
    }

    :global a {
        color: grey;
        text-decoration: none;
    }

    :global a:hover {
        color: #0077b6;
    }

    :global .external-icon {
        display: inline-block;
        width: 1rem;
        height: 1rem;
        --svg: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23000' d='M19 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h6v2H5v12h12v-6zM13 3v2h4.586l-7.793 7.793l1.414 1.414L19 6.414V11h2V3z'/%3E%3C/svg%3E");
        background-color: currentColor;
        -webkit-mask-image: var(--svg);
        mask-image: var(--svg);
        -webkit-mask-repeat: no-repeat;
        mask-repeat: no-repeat;
        -webkit-mask-size: 100% 100%;
        mask-size: 100% 100%;
    }

    .primary {
        background-color: var(--primary );
        padding: 0.5rem 1rem;
        border-radius: 999px;
    }

    .primary:hover {
        background-color: var(--primaryHover );
    }
    
    .primary:active {
        background-color: var(--primaryHover );
        transform: scale(0.95);

    }

    .container {
        align-items: center;
        justify-content: center;
        height: 3rem;
        max-height: 3rem;
        display: flex;
        padding: 0.5rem;
        position: sticky;
        top: 0;
        z-index: 999;
        background-color: var(--surface);
    }
    .content {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 100%;
        max-width: var(--content-width);
        height: 100%;
        max-height: 100%;
    }
    .buttons {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
    :global .nav-button {
        display: flex;
        color: white;
        border: 0;
        padding: 0.5rem 1rem;
        border-radius: 10px;
        text-decoration: none;
        background-color: transparent;
        cursor: pointer;
        transition: 150ms ease;
        white-space: nowrap;
        place-items: center;
        text-align: center;

    }
    :global .nav-button:hover {
        color: white;
        background-color: var(--surfaceHover);
    }

  footer {
    display: flex;
    margin: 0;
    padding: 16px;
    place-items: center;
    margin-top: 60px;
    background-color: var(--surface);
  }

  .footer-text {
    align-self: flex-start;
    padding: 16px;
    display: flex;
    flex-direction: column;
  }

  .footer-links {
    display: flex;
    padding:16px;
  }

  .section-items {
    display: flex;
    width: 100%;
    max-width: var(--content-width);
    margin: 16px auto;
  }

</style>