<script>
	import projects from '../data/projects.js';
</script>

<header>
	<h1>Projects</h1>
</header>
<ul>
	{#each projects as project}
		<li class="project">
			<div class="project__child-container">
				<h2 target="_blank" href={project.url}>
					{project.name}
				</h2>
				<p>{project.description}</p>
			</div>
			<div class="project__child-container">
				<img src={project.src} alt={project.name} />
			</div>
		</li>
	{/each}
</ul>

<style>
	header {
		margin: var(--xl-spacer) 0;
	}
	header h1 {
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
