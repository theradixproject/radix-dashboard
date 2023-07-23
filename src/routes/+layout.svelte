<script>
	import Header from '$lib/components/Header.svelte'
    import Footer from '$lib/components/Footer.svelte'
	// import './styles.css';
	import "../app.css"
</script>

<div class="app bg-black">
	<Header />

	<main>
		<slot />
	</main>

	<Footer />
</div>

<style>
    main {
        min-height: 100vh;
        margin-left: 35px;
        margin-right: 35px;
        color: white !important;
        background-color: black !important;
        display: flex;
        flex-direction: column;
    }

    @media (prefers-color-scheme: light) {
        main {
            color: black !important;
            background-color: white !important;
        }
    }
</style>