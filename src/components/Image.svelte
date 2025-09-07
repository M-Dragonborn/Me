<script lang="ts">
	import { onMount } from 'svelte';
	let cursor;
	let container;
	let active = false;

	onMount(() => {
		const move = (e: MouseEvent) => {
			if (!active) return;
			const rect = container.getBoundingClientRect();
			const x = e.clientX - rect.left;
			const y = e.clientY - rect.top;
			cursor.style.left = `${x}px`;
			cursor.style.top = `${y}px`;
		};

		const enter = () => { active = true; cursor.style.display = 'block'; };
		const leave = () => { active = false; cursor.style.display = 'none'; };

		container.addEventListener('mousemove', move);
		container.addEventListener('mouseenter', enter);
		container.addEventListener('mouseleave', leave);

		return () => {
			container.removeEventListener('mousemove', move);
			container.removeEventListener('mouseenter', enter);
			container.removeEventListener('mouseleave', leave);
		};
	});
</script>

<div class="profile-container" bind:this={container}>
	<img src="pfpmain.webp" alt="M_Dragonborn" />
	<div class="cursor-invert" bind:this={cursor}></div>
</div>

<style lang="scss">
	.profile-container {
		position: relative;
		display: inline-block;
	}

	img {
		cursor: none; /* Hide default cursor when hovering */
		width: 1350px;
		border-radius: 20px;
		animation: hovering 2.5s ease-in-out infinite;
		transition: filter 0.3s ease;
		@media (max-width: 505px) {
			width: 100%;
		}
	}

	.cursor-invert {
		position: absolute;
		width: 80px; /* circle size */
		height: 80px;
		border-radius: 50%;
		backdrop-filter: invert(1);
		-webkit-backdrop-filter: invert(1);
		pointer-events: none;
		transform: translate(-50%, -50%);
		display: none; /* hidden by default */
	}

	@keyframes hovering {
		0% { transform: translateY(6px); }
		50% { transform: translateY(-6px); }
		100% { transform: translateY(6px); }
	}
</style>
