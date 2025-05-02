<script lang="ts">

    const metaImage = "https://www.tellableapp.com/meta_preview.jpg"

</script>

<svelte:head>
    <title>Tellable</title>
    <meta name="author" content="Edgar Martinez" />
    <meta name="description" content="Telling stories is hard, and telling GOOD stories is even harder.
    Tellable takes lets you note down things that happen in your everyday life and turns them into 
    engaging narratives for you to share with friends later. Pick up some of the best ways to tell 
    your stories so that people really tune in when you talk." 
    />
    <meta property="og:title" content="Tellable" />
    <meta property="og:type" content="website" />
    <meta property="og:image" content={metaImage} />
    <meta property="og:description" content="Telling stories is hard, and telling GOOD stories is even harder.
    Tellable takes lets you note down things that happen in your everyday life and turns them into 
    engaging narratives for you to share with friends later. Pick up some of the best ways to tell 
    your stories so that people really tune in when you talk." 
    />
    <meta property="og:url" content="https://www.tellableapp.com" />
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:site" content="@tellable" />
    <meta name="twitter:creator" content="@tellable" />
    <meta name="twitter:image" content={metaImage} />
    <meta name="twitter:description" content="Telling stories is hard, and telling GOOD stories is even harder.
    Tellable takes lets you note down things that happen in your everyday life and turns them into 
    engaging narratives for you to share with friends later. Pick up some of the best ways to tell 
    your stories so that people really tune in when you talk." />
    <meta name="twitter:title" content="Tellable" />
</svelte:head>

<section>

    <div class="items">
        <h1>Tellable App</h1>
        <p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
    </div>

</section>


<style>

    section {
        place-items: center;
        width: 100%;
    }

    .items {
        width: 100%;
        max-width: var(--content-width);
    }

</style>