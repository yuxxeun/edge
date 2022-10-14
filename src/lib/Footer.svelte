<footer>

	<p class="details">
		Built with <a target="_blank" href="https://kit.svelte.dev">SvelteKit</a> +
		<a target="_blank" href="https://github.com/sveltejs/kit/tree/master/packages/adapter-vercel"
			>adapter-vercel</a
		>

		<small>Generated at {new Date().toISOString()}</small>
	</p>
</footer>

<style>
	footer {
		display: grid;
		grid-template-columns: 1fr 1fr;
		align-items: center;
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		text-align: center;
		padding: 2.5rem;
		box-sizing: border-box;
		font-size: 16px;
	}

	p {
		margin: 0.5em 0;
	}

	a {
		color: var(--svelte);
		text-decoration: none;
	}

	a:hover {
		text-decoration: hover;
	}

	.details {
		order: 3;
		grid-column: 1/3;
		white-space: nowrap;
	}

	.source,
	.company {
		display: flex;
		align-items: center;
	}

	.source {
		gap: 0.5rem;
		align-items: center;
		justify-content: flex-end;
	}

	.company {
		font-weight: 600;
		white-space: nowrap;
		justify-content: start;
	}

	.company svg {
		height: 1em;
		position: relative;
		top: 0.2em;
	}

	.source a,
	.company a {
		color: var(--fg);
	}

	small {
		position: absolute;
		left: 0;
		bottom: 20px;
		text-align: center;
		width: 100%;
		font-size: 11px;
		color: #999;
	}

	@media (min-width: 800px) {
		footer {
			display: flex;
			justify-content: space-around;
		}

		.source,
		.company {
			width: 10em;
		}

		.details {
			order: 0;
			grid-column: 1/3;
		}
	}
</style>
