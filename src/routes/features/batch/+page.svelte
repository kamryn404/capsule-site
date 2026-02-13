<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		window.scrollTo(0, 0);
	});
</script>

<svelte:head>
	<title>Batch Processing - Capsule</title>
	<meta name="description" content="Process multiple media files at once with unified settings and organized output." />
</svelte:head>

<div class="container">
	<header class="page-header">
		<a href="/features" class="back-link">← Back to Features</a>
		<h1>Batch Processing</h1>
		<p>Process multiple files at once with unified settings and organized output.</p>
	</header>

	<section class="feature-detail">
		<div class="feature-hero">
			<div class="feature-icon-large">📦</div>
			<h2>Process Multiple Files Efficiently</h2>
			<p>Compress dozens of images, videos, or audio files in one go with consistent settings and organized output.</p>
		</div>

		<div class="feature-sections">
			<section class="feature-section">
				<h3>Key Features</h3>
				<div class="control-list">
					<div class="control-item">
						<div class="control-icon">📁</div>
						<div class="control-content">
							<h4>Multi-File Support</h4>
							<p>Process multiple files at once with drag-and-drop support for easy file selection.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">⚙️</div>
						<div class="control-content">
							<h4>Unified Settings</h4>
							<p>Apply the same compression settings to all files for consistent output quality.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">🖼️</div>
						<div class="control-content">
							<h4>Thumbnail Navigation</h4>
							<p>Horizontal scrollable thumbnail strip for easy file selection and preview.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">📊</div>
						<div class="control-content">
							<h4>Progress Tracking</h4>
							<p>Overall batch progress with individual file progress indicators.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">📂</div>
						<div class="control-content">
							<h4>Organized Output</h4>
							<p>Creates timestamped folders for batch exports, keeping your files organized.</p>
						</div>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Workflow</h3>
				<div class="workflow-steps">
					<div class="workflow-step">
						<div class="step-number">1</div>
						<div class="step-content">
							<h4>Select Files</h4>
							<p>Drag and drop multiple files or use the file picker to select your media.</p>
						</div>
					</div>
					<div class="workflow-step">
						<div class="step-number">2</div>
						<div class="step-content">
							<h4>Configure Settings</h4>
							<p>Set your compression parameters once for all files in the batch.</p>
						</div>
					</div>
					<div class="workflow-step">
						<div class="step-number">3</div>
						<div class="step-content">
							<h4>Preview & Adjust</h4>
							<p>Preview individual files and adjust settings if needed before processing.</p>
						</div>
					</div>
					<div class="workflow-step">
						<div class="step-number">4</div>
						<div class="step-content">
							<h4>Process & Export</h4>
							<p>Start compression and monitor progress. Files are saved to organized folders.</p>
						</div>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Use Cases</h3>
				<div class="use-cases">
					<div class="use-case">
						<h4>Photo Collections</h4>
						<p>Batch process entire photo albums for web sharing or storage optimization.</p>
					</div>
					<div class="use-case">
						<h4>Video Libraries</h4>
						<p>Compress multiple videos for consistent quality across your content library.</p>
					</div>
					<div class="use-case">
						<h4>Audio Archives</h4>
						<p>Optimize music collections or podcast episodes in one go.</p>
					</div>
					<div class="use-case">
						<h4>Asset Preparation</h4>
						<p>Prepare multiple media assets for applications or websites efficiently.</p>
					</div>
				</div>
			</section>
		</div>
	</section>

	<section class="cta-section">
		<h2>Ready to Batch Process Your Files?</h2>
		<p>Download Capsule and start processing multiple files at once.</p>
		<a href="/platforms" class="btn btn-primary">Get Started</a>
	</section>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
		background: linear-gradient(135deg, #0f0f1a 0%, #1a1a2e 50%, #16213e 100%);
		color: #e0e0e0;
		min-height: 100vh;
	}

	.container {
		max-width: 1000px;
		margin: 0 auto;
		padding: 0 20px;
	}

	.page-header {
		text-align: center;
		padding: 60px 20px 40px 20px;
		background: radial-gradient(ellipse at center, rgba(99, 102, 241, 0.1) 0%, transparent 70%);
	}

	.back-link {
		display: inline-block;
		color: #667eea;
		text-decoration: none;
		font-weight: 600;
		margin-bottom: 20px;
		transition: color 0.3s ease;
	}

	.back-link:hover {
		color: #764ba2;
	}

	.page-header h1 {
		font-size: 3rem;
		margin: 0 0 15px 0;
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
	}

	.page-header p {
		font-size: 1.2rem;
		color: #b0b0c0;
		margin: 0;
	}

	.feature-detail {
		padding: 40px 0;
	}

	.feature-hero {
		text-align: center;
		padding: 40px 20px;
		background: rgba(255, 255, 255, 0.05);
		backdrop-filter: blur(10px);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 16px;
		margin-bottom: 40px;
	}

	.feature-icon-large {
		font-size: 5rem;
		margin-bottom: 20px;
	}

	.feature-hero h2 {
		font-size: 2rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.feature-hero p {
		font-size: 1.1rem;
		color: #b0b0c0;
		line-height: 1.6;
		margin: 0;
	}

	.feature-sections {
		display: flex;
		flex-direction: column;
		gap: 40px;
	}

	.feature-section {
		background: rgba(255, 255, 255, 0.03);
		border-radius: 16px;
		padding: 40px;
		border: 1px solid rgba(255, 255, 255, 0.05);
	}

	.feature-section h3 {
		font-size: 1.8rem;
		margin: 0 0 30px 0;
		color: #e0e0e0;
	}

	.control-list {
		display: flex;
		flex-direction: column;
		gap: 20px;
	}

	.control-item {
		display: flex;
		gap: 20px;
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 25px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.control-icon {
		font-size: 2.5rem;
		flex-shrink: 0;
	}

	.control-content h4 {
		font-size: 1.3rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.control-content p {
		color: #b0b0c0;
		line-height: 1.5;
		margin: 0;
	}

	.workflow-steps {
		display: flex;
		flex-direction: column;
		gap: 20px;
	}

	.workflow-step {
		display: flex;
		gap: 20px;
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 25px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.step-number {
		width: 50px;
		height: 50px;
		border-radius: 50%;
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		display: flex;
		align-items: center;
		justify-content: center;
		font-size: 1.5rem;
		font-weight: 700;
		color: white;
		flex-shrink: 0;
	}

	.step-content h4 {
		font-size: 1.3rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.step-content p {
		color: #b0b0c0;
		line-height: 1.5;
		margin: 0;
	}

	.use-cases {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 20px;
	}

	.use-case {
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 25px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.use-case h4 {
		font-size: 1.2rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.use-case p {
		color: #b0b0c0;
		line-height: 1.5;
		margin: 0;
	}

	.cta-section {
		text-align: center;
		padding: 80px 20px;
		background: linear-gradient(135deg, rgba(102, 126, 234, 0.2) 0%, rgba(118, 75, 162, 0.2) 100%);
		border-radius: 16px;
		margin-top: 40px;
	}

	.cta-section h2 {
		font-size: 2rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.cta-section p {
		font-size: 1.1rem;
		color: #b0b0c0;
		margin: 0 0 30px 0;
	}

	.btn {
		display: inline-block;
		padding: 12px 30px;
		border-radius: 8px;
		text-decoration: none;
		font-weight: 600;
		transition: all 0.3s ease;
		border: none;
		cursor: pointer;
		font-size: 1rem;
	}

	.btn-primary {
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		color: white;
		box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
	}

	.btn-primary:hover {
		transform: translateY(-2px);
		box-shadow: 0 6px 20px rgba(102, 126, 234, 0.6);
	}

	@media (max-width: 768px) {
		.page-header h1 {
			font-size: 2rem;
		}

		.feature-hero h2 {
			font-size: 1.5rem;
		}

		.feature-section h3 {
			font-size: 1.5rem;
		}

		.control-item,
		.workflow-step {
			flex-direction: column;
			text-align: center;
		}

		.use-cases {
			grid-template-columns: 1fr;
		}
	}
</style>
