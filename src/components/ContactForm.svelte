<script>
	let name = '';
	let email = '';
	let comments = '';
	let successMessage = '';

	const handleSubmit = async (event) => {
		event.preventDefault();

		const response = await fetch('http://localhost:5000/submit-form', {
			method: 'POST',
			headers: {
				'Content-Type': 'application/json'
			},
			body: JSON.stringify({ name, email, comments })
		});

		if (response.ok) {
			successMessage = 'Message sent successfully';
			name = '';
			email = '';
			comments = '';
		} else {
			successMessage = 'Error sending comments';
		}
	};
</script>

<section class="d-flex align-items-center text-balance" id="contact">
	<div class="container">
		<div class="row justify-content-center">
			<div class="col-md-8 mt-3 text-center">
				<h3>Tailor Us An Email</h3>
				<p class="text-wrap text-dark fw-semibold text-center">
					We are happy to talk you through on how to get started with taking your measurements or
					run live demos for those wishing to see how it's done and what it is to use our services.
				</p>
				<div id="message"></div>
				<form method="post" action="" name="cform" id="cform" on:submit={handleSubmit}>
					<div class="mb-3">
						<input
							name="name"
							id="name"
							type="text"
							class="form-control custom-input"
							placeholder="Your name..."
							bind:value={name}
							required
						/>
					</div>
					<div class="mb-3">
						<input
							name="email"
							id="email"
							type="email"
							class="form-control custom-input"
							placeholder="Email Address..."
							bind:value={email}
							required
						/>
					</div>
					<div class="mb-3">
						<textarea
							name="comments"
							id="comments"
							class="form-control custom-input"
							placeholder="Message Details..."
							bind:value={comments}
							rows="5"
							required
						></textarea>
					</div>
					<div class="text-center mb-3">
						<button type="submit" id="submit" name="send" class="btn btn-primary">Send</button>
					</div>
				</form>
				{#if successMessage}
					<p>{successMessage}</p>
				{/if}
			</div>
		</div>
	</div>
</section>

<style>
	.custom-input {
		border: none;
		border-bottom: 1px solid #ccc;
		border-radius: 0;
	}
	.custom-input:focus {
		box-shadow: none;
		border-bottom: 1px solid #007bff;
	}
</style>
