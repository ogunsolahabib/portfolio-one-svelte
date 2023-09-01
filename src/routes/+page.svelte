<script lang="ts">
	import Header from '../components/Header.svelte';
	import Container from '../components/Container.svelte';
	import Footer from '../components/Footer.svelte';
	import { ThemeWrapper } from 'svelte-theme-switch';
</script>

<ThemeWrapper>
	<Header />
	<Container />
	<Footer />
</ThemeWrapper>
