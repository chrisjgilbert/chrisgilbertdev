<script>
	import projects from '../data/projects.js';
</script>

<header class="header">
	<h1 class="header__copy">Projects</h1>
</header>
<ul>
	{#each projects as project}
		<li class="project">
			<div class="project__card">
				<div class="project__card__child-container">
					<a target="_blank" href={project.url}>
						<h2>{project.name}</h2>
					</a>
					<p>{project.description}</p>
				</div>
				<div class="project__card__child-container">
					<img src={project.src} alt={project.name} />
				</div>
			</div>
		</li>
	{/each}
</ul>

<style>
	.header {
		margin: var(--xl-spacer) 0;
	}
	.header__copy {
		text-align: center;
	}
	.project {
		margin: var(--xl-spacer) 0;
	}

	.project__card {
		display: flex;
		align-items: center;
		grid-gap: var(--l-spacer);
	}
	.project:nth-of-type(even) .project__card {
		flex-direction: row-reverse;
	}

	.project__card__child-container {
		flex: 1;
	}

	.project__card__child-container a {
		color: var(--white);
	}

	.project__card__child-container img {
		height: 100%;
		width: 100%;
	}
</style>
