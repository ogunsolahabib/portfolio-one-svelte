<script lang="ts">
	import { themeStore } from 'svelte-theme-switch';

	const onToggleClick = () =>
		$themeStore.setTheme($themeStore.theme === 'light' ? 'dark' : 'light');
</script>

<header>
	<nav class="main-nav">
		<div class="brand-logo">
			<a href="/">
				<h1>&lt;h/&gt;</h1>
			</a>
		</div>
		<div class="right">
			<div
				role="button"
				class="btn btn--theme-switch"
				aria-labelledby="Switch Theme"
				tabindex="0"
				on:click={onToggleClick}
				on:keydown={onToggleClick}
				on:keypress={onToggleClick}
			/>
			<a
				target="_blank"
				rel="noopener noreferrer"
				href="https://docs.google.com/document/d/e/2PACX-1vSrcUD2WThZGZTSAN1bRfNMy1Zp5ZZEupuMY_xL6X0oc3A3dD5IuYWgq9ftqEVwx4si8zRpOJjCrfWd/pub"
			>
				<button class="btn btn-primary">RESUME</button>
			</a>
		</div>
	</nav>
</header>

<style>
	.brand-logo h1 {
		font-size: 5rem;
		vertical-align: middle;
		text-align: center;
		font-family: 'Dancing Script', cursive, sans-serif;
	}

	.right {
		display: flex;
		align-items: center;
		gap: 2rem;
	}
	.btn--theme-switch {
		aspect-ratio: 1 / 1;
		box-shadow: currentcolor 0px 0px 0px 1px;
		background-image: linear-gradient(270deg, currentcolor 50%, transparent 50%, transparent 100%);
		border-radius: 100%;
		color: var(--text-color);
		width: 2rem;
		height: 2rem;
	}
	.main-nav {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>
