<svelte:head>
	<title>Chris Gilbert | Software Developer - About</title>
</svelte:head>

<div class="about">
	<div class="about__image-container">
		<img class="about__image" src="chrisgilbert.png" alt="chris gilbert" />
	</div>
	<div class="about__copy">
		<p>
			I am a London based Software Devloper currently working at <a
				href="https://multiverse.io/"
				target="_blank">Multiverse</a
			>.
		</p>
		<p>
			Outside of my day job I like to work on <a href="/projects">side projects</a> and write blog posts
			which will eventually live here.
		</p>
	</div>

	<ul>
		<li>
			<a target="_blank" href="https://www.github.com/chrisjgilbert">
				<img class="logo" src="github-logo.png" alt="github" />
			</a>
			<a target="_blank" href="https://www.linkedin.com/in/chrisjgilbert88">
				<img class="logo" src="linkedin-logo.png" alt="linkedin" />
			</a>
			<a href="mailto:chrisjgilbert3@gmail.com">
				<img class="logo" src="email-logo.png" alt="linkedin" />
			</a>
		</li>
	</ul>
</div>

<style>
	.about {
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: var(--xxl-spacer) 0;
	}

	.about__image-container {
		height: 200px;
		width: 200px;
	}

	.about__image {
		height: 100%;
		width: 100%;
	}

	.about__copy {
		text-align: center;
		max-width: 560px;
		margin: var(--l-spacer) auto;
	}

	.about__copy a {
		color: var(--white);
	}

	.logo {
		padding: var(--s-spacer);
		height: 48px;
		width: 48px;
	}
</style>
