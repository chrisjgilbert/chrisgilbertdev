<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
		<li>
			<a href="/">Chris Gilbert | <strong>Software Developer</strong></a>
		</li>
	</ul>
	<!-- <ul> -->
	<!-- <li> -->
	<!-- <a class:active={$page.path === '/projects'} href="/projects">Projects</a> -->
	<!-- </li> -->
	<!-- <li> -->
	<!-- <a class:active={$page.path === '/blog'} href="/blog">Blog</a> -->
	<!-- </li> -->
	<!-- </ul> -->
</nav>

<style>
	nav {
		padding: var(--l-spacer) 0;
		display: flex;
		justify-content: space-between;
		border-bottom: 1px solid var(--white);
	}

	ul {
		display: flex;
		justify-content: space-between;
	}

	li {
		/* padding: 0 var(--s-spacer); */
	}

	a {
		color: var(--white);
		text-decoration: none;
	}

	a.active {
		font-weight: bold;
	}
</style>
