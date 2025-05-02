<script>
    import logo from "$lib/assets/app_icon_cropped_1024.png"
    import word_logo from "$lib/assets/word_logo.png"
</script>

<a class="logo" href="/">
    <!-- <img style="display: flex; max-height: 100%;" src={logo} alt="Tellable App Logo" /> -->
    <img style="display: flex; max-height: 1.5rem;" src={word_logo} alt="Tellable App Logo" />
</a>


<style>
    .logo {
        display: flex;
        height: 100%;
        max-height: 100%;
        flex-direction: row;
        align-items: center;
        gap: 1rem;
    }

    p {
        display: flex;
        white-space: nowrap;
        color: var(--onSurface);
        font-size: 2rem;
        font-weight: bold;
    }
</style>