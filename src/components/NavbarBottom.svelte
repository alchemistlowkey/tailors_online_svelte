<script>
	let isNavOpen = false;
</script>

<nav class="bg-green-500">
	<div class="container mx-auto nav-img2 flex items-center justify-between p-4">
		<a href="/" class="flex items-center">
			<img src="/base/images/logo.png" class="logo" alt="Logo of The Tailors Online" />
		</a>
		<button
			class="text-white block lg:hidden"
			on:click={() => (isNavOpen = !isNavOpen)}
			aria-controls="navbarNav"
			aria-expanded={isNavOpen}
			aria-label="Toggle navigation"
		>
			<svg
				class="w-6 h-6"
				fill="none"
				stroke="currentColor"
				viewBox="0 0 24 24"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M4 6h16M4 12h16M4 18h16"
				></path>
			</svg>
		</button>
		<div
			class={`lg:flex lg:items-center lg:w-auto ${isNavOpen ? 'block' : 'hidden'}`}
			id="navbarNav"
		>
			<ul class="lg:flex lg:justify-end text-green-800 fw-bold fs-6 text-end">
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="/">Home</a>
				</li>
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="/measurement"
						>Get measured</a
					>
				</li>
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="/register">Register</a>
				</li>
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="/login">Login</a>
				</li>
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="#contact">Contact Us</a>
				</li>
				<li class="nav-item">
					<a class="nav-link block px-4 py-2 hover:text-green-600" href="#about">About Us</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

<style>
	.logo {
		max-width: 100px;
	}
	.nav-img2 {
		background-image: url('../lib/img/tailor1.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: center;
		padding: 10px 0;
		width: 100%;
	}
</style>
