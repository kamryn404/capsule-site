<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		window.scrollTo(0, 0);
	});
</script>

<svelte:head>
	<title>Platforms - Capsule</title>
	<meta name="description" content="Download Capsule for Windows, macOS, Linux, Android, and iOS." />
</svelte:head>

<div class="container">
	<header class="page-header">
		<a href="/" class="back-link">← Back to Home</a>
		<h1>Download Capsule</h1>
		<p>Available on all major platforms with consistent experience.</p>
	</header>

	<section class="platforms-section">
		<h2 class="section-title">Choose Your Platform</h2>
		<div class="platforms-grid">
			<div class="platform-card">
				<div class="platform-icon">🪟</div>
				<h3>Windows</h3>
				<p>Full-featured desktop application with drag-and-drop support and custom window management.</p>
				<ul class="platform-features">
					<li>System FFmpeg detection</li>
					<li>Hardware acceleration (NVENC, AMF, QSV)</li>
					<li>Drag & drop support</li>
					<li>Custom titlebar</li>
				</ul>
				<button class="btn btn-primary btn-disabled">Coming Soon</button>
			</div>

			<div class="platform-card">
				<div class="platform-icon">🍎</div>
				<h3>macOS</h3>
				<p>Native macOS experience with VideoToolbox hardware acceleration and hybrid FFmpeg support.</p>
				<ul class="platform-features">
					<li>Hybrid FFmpeg service</li>
					<li>VideoToolbox acceleration</li>
					<li>Native camera integration</li>
					<li>Custom window controls</li>
				</ul>
				<button class="btn btn-primary btn-disabled">Coming Soon</button>
			</div>

			<div class="platform-card">
				<div class="platform-icon">🐧</div>
				<h3>Linux</h3>
				<p>Open-source friendly with automatic distro detection and system FFmpeg integration.</p>
				<ul class="platform-features">
					<li>System FFmpeg detection</li>
					<li>VAAPI hardware acceleration</li>
					<li>Distro-specific instructions</li>
					<li>Drag & drop support</li>
				</ul>
				<button class="btn btn-primary btn-disabled">Coming Soon</button>
			</div>

			<div class="platform-card">
				<div class="platform-icon">🤖</div>
				<h3>Android</h3>
				<p>Full-featured mobile app with gallery integration and bundled FFmpegKit.</p>
				<ul class="platform-features">
					<li>Bundled FFmpegKit</li>
					<li>Gallery save integration</li>
					<li>Camera capture</li>
					<li>Audio recording</li>
				</ul>
				<button class="btn btn-primary btn-disabled">Coming Soon</button>
			</div>

			<div class="platform-card">
				<div class="platform-icon">📱</div>
				<h3>iOS</h3>
				<p>Native iOS experience with Photos integration and bundled FFmpegKit.</p>
				<ul class="platform-features">
					<li>Bundled FFmpegKit</li>
					<li>Photos save integration</li>
					<li>Camera capture</li>
					<li>Audio recording</li>
				</ul>
				<button class="btn btn-primary btn-disabled">Coming Soon</button>
			</div>
		</div>
	</section>

	<section class="requirements-section">
		<h2 class="section-title">System Requirements</h2>
		<div class="requirements-grid">
			<div class="requirement-card">
				<h3>Desktop (Windows/macOS/Linux)</h3>
				<ul>
					<li>FFmpeg installed (auto-detected on most systems)</li>
					<li>2GB RAM minimum, 4GB recommended</li>
					<li>500MB free disk space</li>
					<li>Hardware acceleration requires compatible GPU</li>
				</ul>
			</div>
			<div class="requirement-card">
				<h3>Mobile (Android/iOS)</h3>
				<ul>
					<li>Android 6.0+ / iOS 13.0+</li>
					<li>2GB RAM minimum</li>
					<li>500MB free storage space</li>
					<li>Camera and microphone permissions</li>
				</ul>
			</div>
		</div>
	</section>

	<section class="privacy-section">
		<h2 class="section-title">Privacy & Security</h2>
		<div class="privacy-content">
			<div class="privacy-item">
				<div class="privacy-icon">🔒</div>
				<div class="privacy-text">
					<h3>Local Processing Only</h3>
					<p>All media compression happens locally on your device. No files are uploaded to any server.</p>
				</div>
			</div>
			<div class="privacy-item">
				<div class="privacy-icon">🚫</div>
				<div class="privacy-text">
					<h3>No Data Collection</h3>
					<p>Capsule does not collect, store, or transmit any user data or usage statistics.</p>
				</div>
			</div>
			<div class="privacy-item">
				<div class="privacy-icon">👤</div>
				<div class="privacy-text">
					<h3>No Account Required</h3>
					<p>Use Capsule without creating an account or providing any personal information.</p>
				</div>
			</div>
		</div>
	</section>

	<section class="cta-section">
		<h2>Stay Updated</h2>
		<p>Subscribe to be notified when Capsule is available for your platform.</p>
		<button class="btn btn-primary btn-disabled">Notify Me</button>
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

	.platforms-section {
		padding: 60px 20px;
	}

	.section-title {
		text-align: center;
		font-size: 2.5rem;
		margin: 0 0 50px 0;
		color: #e0e0e0;
	}

	.platforms-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
		gap: 30px;
		max-width: 1200px;
		margin: 0 auto;
	}

	.platform-card {
		background: rgba(255, 255, 255, 0.05);
		backdrop-filter: blur(10px);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 16px;
		padding: 30px;
		text-align: center;
		transition: all 0.3s ease;
	}

	.platform-card:hover {
		transform: translateY(-5px);
		border-color: rgba(102, 126, 234, 0.5);
		box-shadow: 0 10px 30px rgba(102, 126, 234, 0.2);
	}

	.platform-icon {
		font-size: 4rem;
		margin-bottom: 20px;
	}

	.platform-card h3 {
		font-size: 1.8rem;
		margin: 0 0 15px 0;
		color: #e0e0e0;
	}

	.platform-card p {
		color: #b0b0c0;
		line-height: 1.6;
		margin: 0 0 20px 0;
	}

	.platform-features {
		list-style: none;
		padding: 0;
		margin: 0 0 25px 0;
		text-align: left;
	}

	.platform-features li {
		color: #b0b0c0;
		padding: 8px 0;
		padding-left: 25px;
		position: relative;
	}

	.platform-features li:before {
		content: "✓";
		position: absolute;
		left: 0;
		color: #667eea;
		font-weight: bold;
	}

	.requirements-section {
		padding: 60px 20px;
		background: rgba(255, 255, 255, 0.02);
	}

	.requirements-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 30px;
		max-width: 900px;
		margin: 0 auto;
	}

	.requirement-card {
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 30px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.requirement-card h3 {
		font-size: 1.5rem;
		margin: 0 0 20px 0;
		color: #e0e0e0;
	}

	.requirement-card ul {
		list-style: none;
		padding: 0;
		margin: 0;
	}

	.requirement-card li {
		color: #b0b0c0;
		padding: 10px 0;
		padding-left: 25px;
		position: relative;
	}

	.requirement-card li:before {
		content: "•";
		position: absolute;
		left: 0;
		color: #667eea;
		font-weight: bold;
	}

	.privacy-section {
		padding: 60px 20px;
	}

	.privacy-content {
		display: flex;
		flex-direction: column;
		gap: 30px;
		max-width: 900px;
		margin: 0 auto;
	}

	.privacy-item {
		display: flex;
		gap: 20px;
		background: rgba(255, 255, 255, 0.05);
		border-radius: 12px;
		padding: 30px;
		border: 1px solid rgba(255, 255, 255, 0.1);
	}

	.privacy-icon {
		font-size: 3rem;
		flex-shrink: 0;
	}

	.privacy-text h3 {
		font-size: 1.3rem;
		margin: 0 0 10px 0;
		color: #e0e0e0;
	}

	.privacy-text p {
		color: #b0b0c0;
		line-height: 1.5;
		margin: 0;
	}

	.cta-section {
		text-align: center;
		padding: 80px 20px;
		background: linear-gradient(135deg, rgba(102, 126, 234, 0.2) 0%, rgba(118, 75, 162, 0.2) 100%);
		border-radius: 16px;
		margin: 40px 0;
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

	.btn-disabled {
		opacity: 0.5;
		cursor: not-allowed;
	}

	.btn-disabled:hover {
		transform: none;
		box-shadow: none;
	}

	@media (max-width: 768px) {
		.page-header h1 {
			font-size: 2rem;
		}

		.section-title {
			font-size: 2rem;
		}

		.platforms-grid {
			grid-template-columns: 1fr;
		}

		.requirements-grid {
			grid-template-columns: 1fr;
		}

		.privacy-item {
			flex-direction: column;
			text-align: center;
		}
	}
</style>