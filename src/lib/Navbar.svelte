<script>
	export let baslik
	function toggleFunction() {
		var x = document.getElementById('navDemo')
		if (x.className.indexOf('w3-show') == -1) {
			x.className += ' w3-show'
		} else {
			x.className = x.className.replace(' w3-show', '')
		}
	}
</script>

<div class="w3-top" id="Navbar">
	<div class="w3-bar" id="myNavbar">
		<!-- svelte-ignore a11y-invalid-attribute -->
		<div
			on:click={toggleFunction}
			class="w3-bar-item w3-button w3-hover-black w3-hide-medium w3-hide-large w3-right"
			title="Toggle Navigation Menu"
		>
			<i class="fa fa-bars" />
		</div>
		<a href="#home" class="w3-bar-item w3-button" id="homePage">Ana Sayfa</a>
		<a class="w3-bar-item w3-button w3-hide-small" id="navTitle1">{baslik}</a>
		<a href="#yazilarim" class="w3-bar-item w3-button w3-hide-small"
			><i class="fa fa-th" /> Yazılarım</a
		>
		<a href="#iletisim" class="w3-bar-item w3-button w3-hide-small"
			><i class="fa fa-envelope" /> İletişim</a
		>
	</div>

	<!-- Navbar on small screens -->
	<div
		id="navDemo"
		class="w3-bar-block w3-white w3-hide w3-hide-large w3-hide-medium"
	>
		<a class="w3-bar-item w3-button" id="navTitle2" on:click={toggleFunction}
			>Çiçekçi Çocuk</a
		>
		<a href="#yazilarim" class="w3-bar-item w3-button" on:click={toggleFunction}
			>Yazılarım</a
		>
		<a href="#iletisim" class="w3-bar-item w3-button" on:click={toggleFunction}
			>İletişim</a
		>
	</div>
</div>
