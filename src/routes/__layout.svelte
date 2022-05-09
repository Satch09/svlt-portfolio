<script>
	import Navbar from '../components/Navbar.svelte';
import {fade, blur }from 'svelte/transition'

	import '../app.css';
	import NavCenter from '../components/NavCenter.svelte';
	import Footer from '../components/Footer.svelte';
import { onMount } from 'svelte';
import OverallGrid from '../layouts/OverallGrid.svelte';
 let visible = false
	onMount(() => visible = true)
</script>

<!-- <Navbar /> -->

<svelte:head><title>Home</title></svelte:head>

<div class="top">
	<NavCenter />
</div>
<div in:fade>
	<slot />
</div>
<div class="footer">
	<Footer />
</div>

<style></style>
