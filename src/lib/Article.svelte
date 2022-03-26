<script>
	//window.onscroll = function () {
	//	myFunction()
	//}
	function myFunction() {
		var navbar = document.getElementById('myNavbar')
		if (
			document.body.scrollTop > 100 ||
			document.documentElement.scrollTop > 100
		) {
			navbar.className = 'w3-bar' + ' w3-card' + ' w3-animate-top' + ' w3-white'
		} else {
			navbar.className = navbar.className.replace(
				' w3-card w3-animate-top w3-white',
				''
			)
		}
	}
</script>

<div class="bgimg-1 w3-display-container w3-opacity-min" id="home">
	<div class="w3-display-middle" style="white-space:nowrap;">
		<span
			class="w3-center w3-padding-large w3-black w3-xlarge w3-wide w3-animate-opacity"
			id="sahinistambul">Şahin <span class="w3-hide-small" /> İstambul</span
		>
	</div>
</div>

<!-- Container (Yazilarim Section) -->
<div class="w3-content w3-container w3-padding-64" id="baslik">
	<h3 class="w3-center" id="contentTitle">Çiçekçi Çocuk</h3>
	<div class="w3-row">
		<div class="w3-col m6 w3-center w3-padding-large" style="margin-top:7rem">
			<img
				id="contentPic"
				class="w3-round w3-image"
				alt="Content"
				width="500"
				height="333"
			/>
		</div>

		<!-- Hide this text on small devices -->
		<div class="w3-col m6 w3-padding-large">
			<p id="yazi1" />
		</div>
	</div>
	<div class="w3-row w3-container w3-padding-64">
		<p id="yazi2" />
	</div>
</div>
<!-- Second Parallax Image with Portfolio Text -->
<div class="bgimg-2 w3-display-container w3-opacity-min" />

<!-- Container (Portfolio Section) -->
<div class="w3-content w3-container w3-padding-64" id="yazilarim">
	<h3 class="w3-center">Yazılarım</h3>
	<!-- Responsive Grid. Four columns on tablets, laptops and desktops. Will stack on mobile devices/small screens (100% width) -->
	<div id="articles" />
</div>

<!-- Third Parallax Image with Portfolio Text -->
<div class="bgimg-3 w3-display-container w3-opacity-min">
	<div class="w3-display-middle">
		<span class="w3-xxlarge w3-text-white w3-wide">İletişim</span>
	</div>
</div>
