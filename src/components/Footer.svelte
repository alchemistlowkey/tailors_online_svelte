<script>
	let email = '';
	let successMessage = '';

	const handleSubmit = async (event) => {
		event.preventDefault();

		const response = await fetch('http://localhost:5000/subscribe-newsletter', {
			method: 'POST',
			headers: {
				'Content-Type': 'application/json'
			},
			body: JSON.stringify({ email })
		});

		if (response.ok) {
			successMessage = 'Succeccfully subscribed to newsletter';
			email = '';
		} else {
			successMessage = 'Error subscribing to newsletter';
		}
	};
</script>

<footer class="footer footer-bg pt-5 text-green-600 fw-bolder text-balance">
	<!--<div class="action-lage"></div>-->
	<div class="container">
		<div class="row">
			<div class="col-md-4" id="about">
				<h5 class="text-red-700 fw-bold">About Us</h5>
				<p class="mt-2 text-balance fw-semibold">
					We are an online platform that helps people connect to numerous fashion designers/tailors
					out there to get the best out of fashion with ease.
				</p>
				<div class="mt-4">
					<i class="bi-geo-alt text-primary"></i>
					<span class=""> Location: Lagos, Nigeria.</span>
				</div>
				<div class="mt-4">
					<a href="tel:+2348027513561"
						><i class="bi-phone text-primary"></i>
						<span class="">Call us: +234 802 751 3561</span></a
					>
				</div>
				<div class="mt-4">
					<a href="https://wa.me/09035007570"
						><i class="bi-whatsapp text-primary"></i>
						<span class="">WhatsApp us: +234 903 500 7570</span></a
					>
				</div>
				<div class="mt-4">
					<a href="mailto:info@thetailorsonline.com"
						><i class="bi-envelope-plus text-success"></i>
						<span class="">Contact us: info@tailorsonline.tech</span></a
					>
				</div>
				<!-- End of widget item -->
			</div>
			<!-- End of col-md-4 -->

			<div class="col-md-4">
				<div class="widget_item widget_newsletter sm-m-top-50">
					<h5 class="text-red-700 fw-bold">Newsletter</h5>
					<form class="form-inline mt-3" method="post" on:submit={handleSubmit}>
						<div class="form-group d-flex align-items-center">
							<input
								type="email"
								class="form-control border-bottom rounded text-white bg-transparent"
								placeholder="Enter your Email"
								bind:value={email}
							/>
							<button type="submit" class="btn bg-green-600 text-center rounded">
								<i class="bi bi-arrow-right"></i>
							</button>
						</div>
					</form>
					{#if successMessage}
						<p>{successMessage}</p>
					{/if}

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
					<h5 class="text-red-700 fw-bold">Our Services</h5>
					<p><strong>This includes:</strong></p>
					<ul class="list-block m-top-20">
						<li>Access to a large database of fashion designers.</li>
						<br />
						<li>Selling of quality fabrics.</li>
						<br />
						<li>Quality Designs</li>
						<br />
						<li>Fast Delivery</li>
                        <br />
                        <li>Easy Access to Fashion Designers</li>
                        <br />                        
					</ul>
				</div>
				<!-- End off widget item -->
			</div>
			<!-- End off col-md-4 -->
		</div>
	</div>
	<div class=" text-center text-blue-500 pt-4 pb-4 mt-5">
		<div class="col-md-12">
			<p class="" data-wow-duration="1s">
				&copy;2024. Tailors Online. All Rights Reserved.
			</p>
		</div>
	</div>
</footer>

<style>
	.footer-bg {
		background-image: url('../lib/img/tailor6.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: center;
		width: 100%; /* Full width */
	}
</style>
