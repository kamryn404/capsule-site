<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		window.scrollTo(0, 0);
	});
</script>

<svelte:head>
	<title>Features - Capsule</title>
	<meta name="description" content="Explore all features of Capsule media compression application." />
</svelte:head>

<div class="container">
	<header class="page-header">
		<h1>Features</h1>
		<p>Discover everything Capsule has to offer for media compression and optimization.</p>
	</header>

	<nav class="feature-nav">
		<a href="/features/image" class="feature-nav-item">
			<span class="feature-nav-icon">🖼️</span>
			<span class="feature-nav-text">Image Compression</span>
		</a>
		<a href="/features/video" class="feature-nav-item">
			<span class="feature-nav-icon">🎬</span>
			<span class="feature-nav-text">Video Compression</span>
		</a>
		<a href="/features/audio" class="feature-nav-item">
			<span class="feature-nav-icon">🎵</span>
			<span class="feature-nav-text">Audio Compression</span>
		</a>
		<a href="/features/batch" class="feature-nav-item">
			<span class="feature-nav-icon">📦</span>
			<span class="feature-nav-text">Batch Processing</span>
		</a>
	</nav>

	<section class="feature-overview">
		<h2>Why Choose Capsule?</h2>
		<div class="overview-grid">
			<div class="overview-item">
				<h3>🔒 Privacy-First</h3>
				<p>All processing happens locally on your device. No cloud uploads, no data collection. Your media stays yours.</p>
			</div>
			<div class="overview-item">
				<h3>⚡ Performance</h3>
				<p>Hardware acceleration and smart caching ensure fast compression without quality loss.</p>
			</div>
			<div class="overview-item">
				<h3>🌐 Cross-Platform</h3>
				<p>Available on Windows, macOS, Linux, Android, and iOS with a consistent experience.</p>
			</div>
			<div class="overview-item">
				<h3>👁️ Real-Time Preview</h3>
				<p>See before and after comparisons instantly with side-by-side previews.</p>
			</div>
		</div>
	</section>

	<section class="additional-features">
		<h2>Additional Features</h2>
		<div class="features-list">
			<div class="feature-item">
				<h3>Media Capture</h3>
				<p>Built-in camera interface for capturing photos and videos, plus audio recording functionality.</p>
			</div>
			<div class="feature-item">
				<h3>Drag & Drop</h3>
				<p>Desktop drag-and-drop support for single and batch files makes importing media effortless.</p>
			</div>
			<div class="feature-item">
				<h3>Dark Theme</h3>
				<p>Modern dark theme with Material 3 design for comfortable viewing in any lighting.</p>
			</div>
			<div class="feature-item">
				<h3>Responsive Layout</h3>
				<p>Adapts to narrow and wide screens, ensuring a great experience on any device.</p>
			</div>
			<div class="feature-item">
				<h3>File Size Display</h3>
				<p>Shows original vs estimated compressed file sizes so you know exactly what to expect.</p>
			</div>
			<div class="feature-item">
				<h3>Task Cancellation</h3>
				<p>Ability to cancel ongoing compression tasks if you change your mind.</p>
			</div>
		</div>
	</section>

	<section class="cta-section">
		<h2>Ready to Get Started?</h2>
		<p>Download Capsule and start optimizing your media files today.</p>
		<a href="/platforms" class="btn btn-primary">Download Now</a>
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
		max-width: 1200px;
		margin: 0 auto;
		padding: 0 20px;
	}

	.page-header {
		text-align: center;
		padding: 80px 20px 40px 20px;
		background: radial-gradient(ellipse at center, rgba(99, 102, 241, 0.1) 0%, transparent 70%);
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

	.feature-nav {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 20px;
		padding: 40px 20px;
		max-width: 1000px;
		margin: 0 auto;
	}

	.feature-nav-item {
		display: flex;
		align-items: center;
		gap: 15px;
		background: rgba(255, 255, 255, 0.05);
		backdrop-filter: blur(10px);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 12px;
		padding: 25px;
		text-decoration: none;
		color: #e0e0e0;
		transition: all 0.3s ease;
	}

	.feature-nav-item:hover {
		transform: translateY(-5px);
		border-color: rgba(102, 126, 234, 0.5);
		box-shadow: 0 10px 30px rgba(102, 126, 234, 0.2);
	}

	.feature-nav-icon {
		font-size: 2.5rem;
	}

	.feature-nav-text {
		font-size: 1.2rem;
		font-weight: 600;
	}

	.feature-overview {
		padding: 60px 20px;
	}

	.feature-overview h2 {
		text-align: center;
		font-size: 2.5rem;
		margin: 0 0 50px 0;
		color: #e0e0e0;
	}

	.overview-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 30px;
		max-width: 1000px;
		margin: 0 auto;
	}

	.overview-item {
		background: rgba(255, 255, 255, 0.05);
		backdrop-filter: blur(10px);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 12px;
		padding: 30px;
	}

	.overview-item h3 {
		font-size: 1.5rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.overview-item p {
		color: #b0b0c0;
		line-height: 1.6;
		margin: 0;
	}

	.additional-features {
		padding: 60px 20px;
		background: rgba(255, 255, 255, 0.02);
	}

	.additional-features h2 {
		text-align: center;
		font-size: 2.5rem;
		margin: 0 0 50px 0;
		color: #e0e0e0;
	}

	.features-list {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 30px;
		max-width: 1000px;
		margin: 0 auto;
	}

	.feature-item {
		background: rgba(255, 255, 255, 0.05);
		backdrop-filter: blur(10px);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 12px;
		padding: 30px;
	}

	.feature-item h3 {
		font-size: 1.3rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.feature-item p {
		color: #b0b0c0;
		line-height: 1.6;
		margin: 0;
	}

	.cta-section {
		text-align: center;
		padding: 100px 20px;
		background: linear-gradient(135deg, rgba(102, 126, 234, 0.2) 0%, rgba(118, 75, 162, 0.2) 100%);
	}

	.cta-section h2 {
		font-size: 2.5rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.cta-section p {
		font-size: 1.2rem;
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

		.feature-overview h2,
		.additional-features h2,
		.cta-section h2 {
			font-size: 2rem;
		}

		.feature-nav {
			grid-template-columns: 1fr;
		}
	}
</style>
