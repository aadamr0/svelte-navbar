<script lang="ts">
	import Navbar from './navbar.svelte';

	let isOpen: boolean = false;
	const toggleOpen = () => {
		isOpen = !isOpen;
	};
</script>

<header>
    <p>logo</p>
    <button class="open-btn" on:click={toggleOpen}>BO</button>


    <div class="nav-div" class:open={isOpen}>
        <Navbar />
        <button class="close-btn" on:click={toggleOpen}>BC</button>
    </div>
</header>

<style>

    header {
        display: flex;
        justify-content: space-between;
    }

	.nav-div {
        position: fixed;
		visibility: hidden;
		opacity: 0;
		transition-duration: 0.5s;
	}
	.open {
        display: block;
		visibility: visible;
		opacity: 1;
	}

	.close-btn {
		position: fixed;
		top: 3%;
		right: 3%;
	}
</style>
