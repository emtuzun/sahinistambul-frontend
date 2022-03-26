<script>
	import Footer from '../lib/Footer.svelte'
	import Contact from '../lib/Contact.svelte'
	import Navbar from '../lib/Navbar.svelte'
	import Article from '../lib/Article.svelte'
</script>

<svelte:head>
	<title>Sahin Istambul</title>
</svelte:head>

<main>
	<Navbar baslik="Cicekci Cocuk" />
	<Article />
	<Contact />
	<Footer />
</main>
