<script>
	import projects from '../data/projects.js';
</script>

<header class="header">
	<h1 class="header__copy">Projects</h1>
</header>
<ul>
	{#each projects as project}
		<li class="project">
			<div class="project__child-container">
				<a target="_blank" href={project.url}>
					<h2>{project.name}</h2>
				</a>
				<p>{project.description}</p>
			</div>
			<div class="project__child-container">
				<img src={project.src} alt={project.name} />
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
		display: flex;
		align-items: center;
		grid-gap: var(--l-spacer);
	}

	.project__child-container {
		flex: 1;
	}

	.project__child-container a {
		color: var(--white);
	}
	.project__child-container img {
		height: 100%;
		width: 100%;
	}
</style>
