<div class="nav-img">
	<div class="container-fluid p-4">
		<div class="row">
			<div class="col text-start">
				<ul class="list-group text-nowrap">
					<li class="list-item p-2">
						<a href="tel:+2348027513561"
							><i class="bi-phone fs-5 text-primary"></i> 
							<span class="text-dark fs-6 fw-semibold"> Call us: +234 802 751 3561</span></a
						>
					</li>
					<li class="list-item p-2">
						<a href="https://wa.me/09035007570"
							><i class="bi-whatsapp fs-5 text-primary"></i>
							<span class="text-dark fs-6 fw-semibold"> WhatsApp us: +234 903 500 7570</span></a
						>
					</li>
					<li class="list-item p-2">
						<a href="mailto:info@thetailorsonline.com"
							><i class="bi-envelope fs-5 text-success"></i>
							<span class="text-dark fs-6 fw-semibold">Contact us: info@tailorsonline.tech</span></a
						>
					</li>
				</ul>
			</div>
			<div class="col text-end">
				<ul class="list-group">
					<li class="list-item p-2">
						<a class="nav-link" href="https://www.facebook.com/thetailorsonline" target="_blank"
							><i class="bi-facebook fs-5 text-success"></i></a
						>
					</li>
					<li class="list-item p-2">
						<a class="nav-link" href="https://www.instagram.com/thetailorsonline/" target="_blank"
							><i class="bi-instagram fs-5 text-warning"></i></a
						>
					</li>
					<li class="list-item p-2">
						<a class="nav-link" href="https://twitter.com/tailorsonline" target="_blank"
							><i class="bi-twitter fs-5 text-info"></i></a
						>
					</li>
				</ul>
			</div>
		</div>
	</div>
</div>

<nav class="navbar navbar-expand-lg navbar-light bg-success">
	<div class="container-fluid nav-img2">
		<a class="navbar-brand" href="/">
			<img src="/base/images/logo.png" class="logo" alt="Logo of The Tailors Online" />
		</a>
		<button
			class="navbar-toggler me-2"
			type="button"
			data-bs-toggle="collapse"
			data-bs-target="#navbarNav"
			aria-controls="navbarNav"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
			<span class="navbar-toggler-icon"></span>
		</button>
		<div class="collapse navbar-collapse" id="navbarNav">
			<ul class="navbar-nav ms-auto text-end pe-2 fw-semibold">
				<li class="nav-item">
					<a class="nav-link" href="/">Home</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/measurement">Get measured</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/register">Register</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/login">Login</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#contact">Contact Us</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#about">About Us</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

<slot />

<footer class="footer footer-bg pt-5">
	<!--<div class="action-lage"></div>-->
	<div class="container">
		<div class="row">
			<div class="col-md-4" id="about">
				<h5 class="text-white">About Us</h5>
				<p class="mt-2 text-secondary fw-semibold">
					We are an online platform that helps people connect to numerous fashion designers/tailors
					out there to get the best out of fashion with ease.
				</p>
				<div class="mt-4">
					<i class="bi-geo-alt text-primary"></i>
					<span class="text-secondary fw-semibold"> Location: Lagos, Nigeria.</span>
				</div>
				<div class="mt-4">
					<a href="tel:+2348027513561"
						><i class="bi-phone text-primary"></i>
						<span class="text-secondary fw-semibold">Call us: +234 802 751 3561</span></a
					>
				</div>
				<div class="mt-4">
					<a href="https://wa.me/09035007570"
						><i class="bi-whatsapp text-primary"></i>
						<span class="text-secondary fw-semibold">WhatsApp us: +234 903 500 7570</span></a
					>
				</div>
				<div class="mt-4">
					<a href="mailto:info@thetailorsonline.com"
						><i class="bi-envelope-plus text-success"></i>
						<span class="text-secondary fw-semibold">Contact us: info@tailorsonline.tech</span></a
					>
				</div>
				<!-- End of widget item -->
			</div>
			<!-- End of col-md-4 -->

			<div class="col-md-4">
				<div class="widget_item widget_newsletter sm-m-top-50">
					<h5 class="text-white">Newsletter</h5>
					<form class="form-inline mt-3" method="post" action="">
						<div class="form-group d-flex align-items-center">
							<input
								type="email"
								class="form-control border-bottom rounded text-white bg-transparent"
								placeholder="Enter your Email"
							/>
							<button type="submit" class="btn text-center rounded">
								<i class="bi bi-arrow-right"></i>
							</button>
						</div>
					</form>

					<ul class="list-inline m-top-20">
						<li>
							<a href="https://www.facebook.com/" target="_blank"><i class="fa fa-facebook"></i></a>
						</li>
						<li>
							<a href="https://www.instagram.com/" target="_blank"
								><i class="fa fa-instagram"></i></a
							>
						</li>
						<li>
							<a href="https://twitter.com/" target="_blank"><i class="fa fa-twitter"></i></a>
						</li>
					</ul>
				</div>
				<!-- End off widget item -->
			</div>
			<!-- End off col-md-4 -->

			<div class="col-md-4">
				<div class="widget_item sm-m-top-50">
					<h5 class="text-white">Our Services</h5>
					<p><strong>This includes:</strong></p>
					<ul class="list-block m-top-20">
						<li>Access to a large database of fashion designers.</li>
						<br />
						<li>Selling of quality fabrics.</li>
						<br />
						<li>Quality Designs</li>
						<br />
						<li></li>
						<li></li>
						<li></li>
						<li></li>
					</ul>
				</div>
				<!-- End off widget item -->
			</div>
			<!-- End off col-md-4 -->
		</div>
	</div>
	<div class=" text-center pt-4 pb-4 mt-5">
		<div class="col-md-12">
			<p class="text-secondary fw-semibold" data-wow-duration="1s">
				&copy;2024. Tailors Online. All Rights Reserved.
			</p>
		</div>
	</div>
</footer>

<style>
	.nav-img {
		background-image: url('../lib/img/tailor2.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: center;
		width: 100%; /* Full width */
	}
	.logo {
		max-width: 100px;
		margin: 0 auto;
	}
	.nav-img2 {
		background-image: url('../lib/img/tailor1.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: center;
		padding: 10px 0;
		width: 100%; /* Full width */
	}
	.footer-bg {
		background-image: url('../lib/img/tailor6.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: center;
		width: 100%; /* Full width */
	}
	.nav-link {
		text-decoration: none;
		color: #000; /* Ensure the text color is readable */
	}
	.nav-link:hover {
		color: #369c1c; /* Optional: Change text color on hover */
	}
	.navbar-light .navbar-toggler-icon {
		background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3E%3Cpath stroke='rgba%280, 0, 0, 0.5%29' stroke-width='2' linecap='round' linejoin='round' d='M4 7h22M4 15h22M4 23h22'/%3E%3C/svg%3E");
	}
</style>
