<script>
import { onMount } from 'svelte';

	import {fade} from 'svelte/transition'
import HeroLayout from '../layouts/HeroLayout.svelte';
	let visible = false
	onMount(() => visible = !visible)

</script>

<HeroLayout>
	<div class="hero hro bg-slate-300  rounded-lg shadow-lg">
		<div class="flex-col lg:flex-row  ">
			<div class="bg-base-200 shadow-md  flex justify-start md:w-1/4 mt-10 absolute top-10 right-5">
				<div class="bg-base-200 mt-10">
					{#if visible}
						<div transition:fade={{delay: 150, duration: 300}}>
							<div transition:fade={{delay: 500, duration: 800}}>
								<h3 class="text-3xl font-bold  m-4 mr-0 pl-2 pr-1">Compliance</h3>
							</div>
							<div transition:fade={{delay: 1300, duration: 800}}>
								<h3 class="text-3xl font-bold  m-4 mr-0 pl-2 pr-1">Reliance</h3>
							</div>
							<div transition:fade={{delay: 2300, duration: 800}}>
								<h3 class="text-3xl font-bold  m-4 mr-0 pl-2 pr-1">Assured</h3>
							</div>
						</div>
						<div class="">
							<div transition:fade={{delay: 3600, duration: 300}}>
								<h1 class="text-5xl font-bold pt-5 md:w-1/4 m-4 mr-0 pl-6 pr-1">DigiComply</h1>
							</div>
						</div>
					{/if}
				</div>
			</div>
		</div>
	</div>
</HeroLayout>

<style>
	.hro {
		justify-content: center;
		min-height: 70vh;

		/* max-height: 60vh; */
	}
</style>
