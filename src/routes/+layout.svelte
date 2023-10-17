<script>
	import { browser } from '$app/environment';
	import '../global.css';

	const meta = {
		title: "Habib Ogunsola's Portfolio website",
		description:
			'Habib is a Frontend Engineer with experience in building aesthetically pleasing large scale web applications',
		keywords:
			'Frontend, Front End, Front-End, Developer, Software Engineer, Web, Habib, Ogunsola, Martial Arts, Lagos, Nigeria, Glasgow, JavaScript, TypeScript, React.js, Svelte'
	};
</script>

<svelte:head>
	<title>{meta.title}</title>
	<meta charset="utf-8" />
	<meta content="width=device-width,initial-scale=1" name="viewport" />
	<base href="/" />
	<link
		href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@300;400;600&amp;display=swap"
		rel="stylesheet"
	/>

	<meta content={meta.keywords} name="keywords" />
	<meta content={meta.title} property="og:title" />
	<meta content="en_GB" property="og:locale" />
	<meta content="website" property="og:type" />
	<meta content="https://habib.ogunsola.me" property="og:url" />
	<meta content="logo-512.png" property="og:image" />
	<meta content="512" property="og:image:width" />
	<meta content="512" property="og:image:height" />
	<meta content={meta.title} property="og:site_name" />
	<meta content={meta.description} name="description" property="og:description" />
	<meta content="summary_large_image" name="twitter:card" />
	<meta content="@ha_beeeb" name="twitter:creator" />
	<meta content={meta.title} name="twitter:title" />
	<meta content={meta.description} name="twitter:description" />
	<meta name="google-site-verification" content="4K3GVII94Nt2n06PhsfrzWsef6ui5dT6aA3C7SeWh0s" />
	<!-- Google Tag Manager -->
	<!-- Google Tag Manager -->
	<!-- Google Tag Manager -->
	<!-- Google Tag Manager -->
	<!-- Google Tag Manager -->
	<!-- Google Tag Manager -->
	<script>
		(function (w, d, s, l, i) {
			w[l] = w[l] || [];
			w[l].push({ 'gtm.start': new Date().getTime(), event: 'gtm.js' });
			var f = d.getElementsByTagName(s)[0],
				j = d.createElement(s),
				dl = l != 'dataLayer' ? '&l=' + l : '';
			j.async = true;
			j.src = 'https://www.googletagmanager.com/gtm.js?id=' + i + dl;
			f.parentNode.insertBefore(j, f);
		})(window, document, 'script', 'dataLayer', 'GTM-5L7WGSSH');
	</script>
	<!-- End Google Tag Manager -->
</svelte:head>

<!-- Google Tag Manager (noscript) -->
<noscript
	><iframe
		title="Google Tag Manager (noscript)"
		src="https://www.googletagmanager.com/ns.html?id=GTM-5L7WGSSH"
		height="0"
		width="0"
		style="display:none;visibility:hidden"
	/></noscript
>
<!-- End Google Tag Manager (noscript) -->
{#if browser}
	<!-- End Google Tag Manager -->
	<!-- End Google Tag Manager -->
	<script async src="https://www.googletagmanager.com/gtag/js?id=G-N30T60DW8P"></script>
	<script>
		window.dataLayer = window.dataLayer || [];
		function gtag() {
			dataLayer.push(arguments);
		}
		gtag('js', new Date());

		gtag('config', 'G-N30T60DW8P');
	</script>
{/if}
<slot />
