<script>
	import Navbar from '../components/Navbar.svelte';

	import '../app.css';
	import NavCenter from '../components/NavCenter.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<NavCenter />
<Navbar />
<slot />
<Footer />
