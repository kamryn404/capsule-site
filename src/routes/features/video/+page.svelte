<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		window.scrollTo(0, 0);
	});
</script>

<svelte:head>
	<title>Video Compression - Capsule</title>
	<meta name="description" content="Compress videos to H.264, H.265, AV1, or VP9 with hardware acceleration and real-time preview." />
</svelte:head>

<div class="container">
	<header class="page-header">
		<a href="/features" class="back-link">← Back to Features</a>
		<h1>Video Compression</h1>
		<p>Powerful video compression with hardware acceleration and real-time preview.</p>
	</header>

	<section class="feature-detail">
		<div class="feature-hero">
			<div class="feature-icon-large">🎬</div>
			<h2>Compress Any Video Format</h2>
			<p>Support for MP4, WebM, MKV, MOV, AVI, FLV, WMV, M4V, TS, and 3GP formats with intelligent codec selection.</p>
		</div>

		<div class="feature-sections">
			<section class="feature-section">
				<h3>Output Formats & Codecs</h3>
				<div class="format-grid">
					<div class="format-card">
						<h4>H.264 (MP4)</h4>
						<p>Universal compatibility with excellent compression. Perfect for web and mobile playback.</p>
					</div>
					<div class="format-card">
						<h4>H.265 (MP4)</h4>
						<p>Next-generation codec with superior compression ratios. Smaller files at same quality.</p>
					</div>
					<div class="format-card">
						<h4>AV1 (MP4)</h4>
						<p>Cutting-edge codec with exceptional efficiency. Best quality at smallest file sizes.</p>
					</div>
					<div class="format-card">
						<h4>VP9 (WebM)</h4>
						<p>Open-source codec with excellent compression. Great for web optimization.</p>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Hardware Acceleration</h3>
				<div class="control-list">
					<div class="control-item">
						<div class="control-icon">⚡</div>
						<div class="control-content">
							<h4>Automatic Detection</h4>
							<p>Automatically detects and uses available hardware encoders for faster compression.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">🖥️</div>
						<div class="control-content">
							<h4>VideoToolbox</h4>
							<p>macOS hardware acceleration for H.264 and H.265 encoding.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">🎮</div>
						<div class="control-content">
							<h4>NVENC</h4>
							<p>NVIDIA GPU acceleration for blazing-fast video compression.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">🔧</div>
						<div class="control-content">
							<h4>AMF / QSV / VAAPI</h4>
							<p>AMD, Intel, and Linux hardware acceleration support.</p>
						</div>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Compression Controls</h3>
				<div class="control-list">
					<div class="control-item">
						<div class="control-icon">🎚️</div>
						<div class="control-content">
							<h4>Bitrate Control</h4>
							<p>Adjustable bitrate with automatic max bitrate detection from source video.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">📐</div>
						<div class="control-content">
							<h4>Resolution Scaling</h4>
							<p>Scale videos to 100%, 50%, or 25% of original resolution for additional size reduction.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">👁️</div>
						<div class="control-content">
							<h4>Real-Time Preview</h4>
							<p>Synchronized composite video showing original (left) vs compressed (right) with pan/zoom support.</p>
						</div>
					</div>
					<div class="control-item">
						<div class="control-icon">📊</div>
						<div class="control-content">
							<h4>Progress Tracking</h4>
							<p>Real-time progress indicator during compression with estimated time remaining.</p>
						</div>
					</div>
				</div>
			</section>

			<section class="feature-section">
				<h3>Use Cases</h3>
				<div class="use-cases">
					<div class="use-case">
						<h4>Web Optimization</h4>
						<p>Compress videos for faster website loading and streaming without quality loss.</p>
					</div>
					<div class="use-case">
						<h4>Social Media</h4>
						<p>Optimize videos for YouTube, Instagram, TikTok, and other platforms.</p>
					</div>
					<div class="use-case">
						<h4>Storage Management</h4>
						<p>Reduce video file sizes to free up disk space while maintaining quality.</p>
					</div>
					<div class="use-case">
						<h4>Proxy Files</h4>
						<p>Create lightweight proxy files for video editing workflows.</p>
					</div>
				</div>
			</section>
		</div>
	</section>

	<section class="cta-section">
		<h2>Ready to Compress Your Videos?</h2>
		<p>Download Capsule and start optimizing your videos today.</p>
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
		.use-cases {
			grid-template-columns: 1fr;
		}
	}
</style>
