<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		window.scrollTo(0, 0);
	});
</script>

<svelte:head>
	<title>Image Compression - Capsule</title>
	<meta name="description" content="Compress images to JPEG, PNG, WEBP, or AVIF with adjustable quality and real-time preview." />
</svelte:head>

<div class="container">
	<header class="page-header">
		<a href="/features" class="back-link">← Back to Features</a>
		<h1>Image Compression</h1>
		<p>Optimize your images with powerful compression tools and real-time preview.</p>
	</header>

	<section class="feature-detail">
		<div class="feature-hero">
			<div class="feature-icon-large">🖼️</div>
			<h2>Compress Any Image Format</h2>
			<p>Support for JPEG, PNG, WEBP, AVIF, HEIC, BMP, TIFF, and GIF formats with intelligent conversion options.</p>
		</div>

		<div class="feature-sections">
			<section class="feature-section">
				<h3>Output Formats</h3>
				<div class="format-grid">
					<div class="format-card">
						<h4>JPEG</h4>
						<p>Universal compatibility with excellent compression ratios. Perfect for photos and web images.</p>
					</div>
					<div class="format-card">
						<h4>PNG</h4>
						<p>Lossless compression with transparency support. Ideal for graphics and logos.</p>
					</div>
					<div class="format-card">
						<h4>WEBP</h4>
						<p>Modern format with superior compression and transparency. Best for web optimization.</p>
					</div>
					<div class="format-card">
						<h4>AVIF</h4>
						<p>Next-generation format with exceptional quality at smaller file sizes.</p>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Quality Control</h3>
				<div class="control-list">
					<div class="control-item">
						<div class="control-icon">🎚️</div>
						<div class="control-content">
							<h4>Adjustable Quality Slider</h4>
							<p>Fine-tune compression from 1-100% to find the perfect balance between file size and quality.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">📐</div>
						<div class="control-content">
							<h4>Resolution Scaling</h4>
							<p>Scale images to 100%, 50%, or 25% of original dimensions for additional size reduction.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">👁️</div>
						<div class="control-content">
							<h4>Real-Time Preview</h4>
							<p>Side-by-side before/after comparison with draggable slider for instant feedback.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">✨</div>
						<div class="control-content">
							<h4>Transparency Support</h4>
							<p>Preserves alpha channel for WEBP and AVIF formats, maintaining transparent backgrounds.</p>
						</div>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Smart Features</h3>
				<div class="smart-features">
					<div class="smart-feature">
						<h4>🔄 Automatic Conversion</h4>
						<p>Smart conversion of HEIC and AVIF to PNG for preview compatibility while preserving original format options.</p>
					</div>
					<div class="smart-feature">
						<h4>⚡ Debounced Preview</h4>
						<p>Optimized preview generation with 500ms debounce for smooth performance even with large images.</p>
					</div>
					<div class="smart-feature">
						<h4>📊 File Size Display</h4>
						<p>Shows original vs estimated compressed file sizes so you know exactly what to expect.</p>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Use Cases</h3>
				<div class="use-cases">
					<div class="use-case">
						<h4>Web Optimization</h4>
						<p>Reduce image sizes for faster website loading without sacrificing visual quality.</p>
					</div>
					<div class="use-case">
						<h4>Social Media</h4>
						<p>Compress images for Instagram, Facebook, Twitter, and other platforms with optimal settings.</p>
					</div>
					<div class="use-case">
						<h4>Storage Management</h4>
						<p>Free up disk space by compressing photo collections while maintaining quality.</p>
					</div>
					<div class="use-case">
						<h4>Email Attachments</h4>
						<p>Reduce image sizes to meet email attachment limits without visible quality loss.</p>
					</div>
				</div>
			</section>
		</div>
	</section>

	<section class="cta-section">
		<h2>Ready to Compress Your Images?</h2>
		<p>Download Capsule and start optimizing your images today.</p>
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

	.format-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 20px;
	}

	.format-card {
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 25px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.format-card h4 {
		font-size: 1.3rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.format-card p {
		color: #b0b0c0;
		line-height: 1.5;
		margin: 0;
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

	.smart-features {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 20px;
	}

	.smart-feature {
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 25px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.smart-feature h4 {
		font-size: 1.3rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.smart-feature p {
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

		.control-item {
			flex-direction: column;
			text-align: center;
		}

		.format-grid,
		.smart-features,
		.use-cases {
			grid-template-columns: 1fr;
		}
	}
</style>
