<script>
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
</svelte:head>
<slot />
