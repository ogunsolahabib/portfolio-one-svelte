<script>
	let projects = [
		{
			name: 'Tunez',
			image: 'Tunez.png',
			description:
				'Frontend App to search songs, artists and albums from the iTunes API. I used TypeScript, React, Express, Jest.',
			repository: 'https://github.com/ogunsolahabib/tunez'
		},
		{
			name: 'REST Countries',
			image: 'REST_COUNTRIES.png',
			description:
				'The web app shows information of 250 countries and has a light theme and dark theme. I built it using ReactJS and Semantic UI',
			repository: 'https://github.com/ogunsolahabib/world-countries',
			liveWebsite: 'https://ogunsolahabib.github.io/world-countries'
		}
	];
	let socials = [
		{
			name: 'GitHub',
			icon: 'fab fa-github',
			link: 'https://github.com/ogunsolahabib'
		},
		{
			name: 'Linkedin',
			icon: 'fab fa-linkedin',
			link: 'https://linkedin.com/in/habibogunsola'
		},
		{
			name: 'Twitter',
			link: 'https://twitter.com/ha_beeeb'
		},
		{
			name: 'Email',
			link: 'mailto:ogunsolahabib@yahoo.com'
		}
	];
</script>

<main class="me">
	<section class="section section--hero">
		<div class="hero__about">
			<h1 class="greeting">
				<span class="greeting__hi">Hi, I'm</span>
				<span class="greeting__name">HABIB OGUNSOLA.</span>
			</h1>
			<div class="description">
				<p>
					A creative Frontend Engineer and UX enthusiast with experience in building aesthetically
					pleasing large scale web applications.
				</p>
				<p>Interested in Tech, Business, Combat sports, and Football.</p>
				<br />
				<p>
					I am currently building User Interfaces with awesome people at{' '}
					<a target="_blank" rel="noreferrer" href="https://www.ahroscientific.com/">
						AHRO Publishing.
					</a>
				</p>
			</div>
		</div>
	</section>
	<section class="section bottom">
		<div id="contact">
			<div>
				<ul class="set social">
					{#each socials as social}
						<li>
							<a target="_blank" rel="noopener noreferrer" href={social.link}>
								<i class={social.icon} /> <span>{social.name}</span>
							</a>
						</li>
					{/each}
				</ul>
			</div>
		</div>
	</section>
</main>

<style>
	.greeting {
		font-size: clamp(2.5rem, 7vmin, 10rem);
		display: flex;
		flex-wrap: wrap;
		gap: 1rem;
	}

	.greeting__hi {
		font-weight: 300;
	}
	.greeting__name {
		font-weight: 600;
	}

	main {
		min-height: 70vh;
		@media screen and (min-width: 768px) {
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
		}
	}

	.description p {
		font-size: clamp(1.5rem, 5vmin, 2.5rem);
	}
	section {
		width: clamp(200px, 100%, 1080px);
		margin: auto;
	}
	#contact {
		margin: auto;
	}
	.social {
		display: flex;
		gap: clamp(10px, 5vw, 30px);
		flex-wrap: wrap;
		margin-top: 50px;
		font-size: clamp(13px, 3vmax, 20px);
	}
	.social a {
		text-decoration: underline;
		padding-bottom: 10px;
	}
</style>
