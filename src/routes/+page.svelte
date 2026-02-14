<script lang="ts">
    const features = [
        {
            title: "Image Compression",
            description:
                "Compress to JPEG, PNG, WEBP, or AVIF with adjustable quality (1-100%) and resolution scaling. Preserve transparency for WEBP and AVIF.",
            icon: "🖼️",
        },
        {
            title: "Video Compression",
            description:
                "Output to H.264, H.265, AV1, or VP9 with hardware acceleration. Adjustable bitrate and resolution scaling with real-time preview.",
            icon: "🎬",
        },
        {
            title: "Audio Compression",
            description:
                "Compress to MP3, Vorbis (OGG), or Opus with adjustable bitrate (32-320 kbps). Preview any segment with side-by-side comparison.",
            icon: "🎵",
        },
        {
            title: "Batch Processing",
            description:
                "Process multiple files at once with unified settings. Thumbnail navigation and organized timestamped output folders.",
            icon: "📦",
        },
        {
            title: "Privacy-First",
            description:
                "All processing happens locally on your device. No cloud uploads, no data collection. Your media stays yours.",
            icon: "🔒",
        },
        {
            title: "Cross-Platform",
            description:
                "Available on Windows, macOS, Linux (Android coming soon). Consistent experience across all platforms.",
            icon: "⚡",
        },
    ];

    const changelog = [
        { title: "Support for AVIF and HEIC images", date: "MAY 1, 2024" },
        { title: "Hardware accelerated AV1 encoding", date: "APR 25, 2024" },
        { title: "Batch processing improvements", date: "APR 25, 2024" },
        { title: "New Opus audio encoder", date: "APR 10, 2024" },
        { title: "MacOS and Windows stable release", date: "APR 9, 2024" },
    ];
</script>

<svelte:head>
    <title>Capsule — Compress. Optimize. Share.</title>
</svelte:head>

<div class="page-wrapper">
    <!-- Hero Section -->
    <section class="hero">
        <h1 class="hero-title">
            Compress.<br />
            Optimize. Share.
        </h1>

        <p class="hero-subtitle">
            A cross-platform application for compressing and optimizing media
            files.<br />
            Process images, videos, and audio with hardware acceleration.
        </p>

        <div class="hero-visual">
            <div class="video-container">
                <video
                    src="/video.mp4"
                    autoplay
                    loop
                    muted
                    playsinline
                    class="hero-video"
                ></video>
            </div>
        </div>
    </section>

    <!-- Features Grid -->
    <section id="features" class="features">
        <div class="grid-container">
            {#each features as feature}
                <div class="feature-card">
                    <div class="feature-icon-box">
                        <span class="icon">{feature.icon}</span>
                    </div>
                    <h3 class="feature-title">{feature.title}</h3>
                    <p class="feature-description">{feature.description}</p>
                </div>
            {/each}
        </div>
    </section>

    <!-- Supported Formats -->
    <section id="formats" class="formats">
        <h2 class="section-title-serif">Supported Formats</h2>
        <div class="formats-grid">
            <div class="format-card">
                <h3>🖼️ Images</h3>
                <p>JPEG, PNG, WEBP, AVIF, HEIC, BMP, TIFF, GIF</p>
            </div>
            <div class="format-card">
                <h3>🎬 Videos</h3>
                <p>MP4, WebM, MKV, MOV, AVI, FLV, WMV, M4V, TS, 3GP</p>
            </div>
            <div class="format-card">
                <h3>🎵 Audio</h3>
                <p>MP3, AAC, OGG, WAV, FLAC, M4A, Opus, AIFF, WMA</p>
            </div>
        </div>
    </section>

    <!-- Use Cases -->
    <section class="use-cases">
        <h2 class="section-title-serif">Perfect For</h2>
        <div class="use-cases-grid">
            <div class="use-case-item">
                <h4>Content Creators</h4>
                <p>
                    Compress media for web and social media sharing without
                    quality loss.
                </p>
            </div>
            <div class="use-case-item">
                <h4>Developers</h4>
                <p>Optimize assets for applications and websites.</p>
            </div>
            <div class="use-case-item">
                <h4>Photographers</h4>
                <p>Batch process image collections efficiently.</p>
            </div>
            <div class="use-case-item">
                <h4>Video Editors</h4>
                <p>Create proxy files for editing workflows.</p>
            </div>
            <div class="use-case-item">
                <h4>General Users</h4>
                <p>Reduce file sizes for storage and sharing.</p>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="download" class="cta">
        <h2 class="section-title-serif">Download</h2>
        <div class="cta-buttons">
            <a
                href="https://github.com/kamryn404/Capsule/releases/latest/download/Capsule.dmg"
                class="cta-button secondary platform-btn"
            >
                <img src="/apple.svg" alt="Mac" class="platform-icon" />
                Mac
            </a>
            <a
                href="https://github.com/kamryn404/Capsule/releases/latest/download/Capsule.exe"
                class="cta-button secondary platform-btn"
            >
                <img src="/windows.svg" alt="Windows" class="platform-icon" />
                Windows
            </a>
            <a
                href="https://github.com/kamryn404/Capsule/releases/latest/download/Capsule.AppImage"
                class="cta-button secondary platform-btn"
            >
                <img src="/linux.svg" alt="Linux" class="platform-icon" />
                Linux
            </a>
        </div>
    </section>

    <footer class="footer">
        <p>&copy; 2026 Capsule</p>
    </footer>
</div>

<style>
    .page-wrapper {
        padding: 120px 20px 0px 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background: radial-gradient(
            circle at 50% -20%,
            #2d1b4e 0%,
            #050505 50%
        );
    }

    /* Hero */
    .hero {
        text-align: center;
        max-width: 900px;
        padding: 0 20px;
        margin-bottom: 120px;
    }

    .hero-title {
        font-family: var(--font-heading);
        font-size: clamp(2.5rem, 6vw, 4rem);
        line-height: 1.1;
        font-weight: 400;
        margin: 0 0 32px 0;
        letter-spacing: -0.02em;
    }

    .hero-subtitle {
        font-size: clamp(1.1rem, 2vw, 1.25rem);
        color: var(--text-secondary);
        line-height: 1.5;
        margin-bottom: 64px;
    }

    .hero-visual {
        width: 100%;
        max-width: 1000px;
        margin: 0 auto;
        position: relative;
        padding: 1px;
        border-radius: 24px;
        box-shadow: 0 0 100px rgba(139, 92, 246, 0.5);
        display: flex;
        justify-content: center;
    }

    .video-container {
        width: 100%;
        max-width: 800px;
        border-radius: 12px;
        overflow: hidden;
        box-shadow: 0 40px 100px rgba(0, 0, 0, 0.8);
        line-height: 0;
    }

    .hero-video {
        width: 100%;
        height: auto;
        display: block;
    }

    /* Features Grid */
    .features {
        width: 100%;
        max-width: 1100px;
        padding: 120px 40px;
    }

    .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 64px 48px;
    }

    .feature-card {
        display: flex;
        flex-direction: column;
        gap: 16px;
    }

    .feature-icon-box {
        width: 32px;
        height: 32px;
        background: rgba(255, 255, 255, 0.05);
        border-radius: 8px;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .icon {
        font-size: 1rem;
    }

    .feature-title {
        font-family: var(--font-heading);
        font-size: 1rem;
        font-weight: 400;
        margin: 0;
        letter-spacing: -0.01em;
    }

    .feature-description {
        font-size: 0.95rem;
        color: var(--text-secondary);
        line-height: 1.5;
        margin: 0;
    }

    .section-title-serif {
        font-family: var(--font-heading);
        font-size: clamp(2.2rem, 5vw, 3.5rem);
        font-weight: 400;
        margin-bottom: 48px;
        letter-spacing: -0.02em;
    }

    /* Formats Section */
    .formats {
        width: 100%;
        max-width: 1100px;
        padding: 80px 40px;
        text-align: center;
    }

    .formats-grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 32px;
    }

    .format-card {
        background: rgba(255, 255, 255, 0.03);
        border: 1px solid rgba(255, 255, 255, 0.05);
        border-radius: 16px;
        padding: 32px;
        text-align: left;
    }

    .format-card h3 {
        font-size: 1.2rem;
        margin: 0 0 12px 0;
    }

    .format-card p {
        color: var(--text-secondary);
        font-size: 0.9rem;
        line-height: 1.6;
        margin: 0;
    }

    /* Use Cases Section */
    .use-cases {
        width: 100%;
        max-width: 1100px;
        padding: 80px 40px;
        text-align: center;
    }

    .use-cases-grid {
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        gap: 24px;
    }

    .use-case-item {
        text-align: left;
    }

    .use-case-item h4 {
        font-size: 1rem;
        margin: 0 0 8px 0;
        color: var(--text-primary);
    }

    .use-case-item p {
        font-size: 0.85rem;
        color: var(--text-secondary);
        line-height: 1.5;
        margin: 0;
    }

    /* CTA Section */
    .cta {
        width: 100%;
        max-width: 1100px;
        padding: 50px 40px;
        text-align: center;
        background: linear-gradient(
            180deg,
            rgba(139, 92, 246, 0.2) 0%,
            transparent 100%
        );
        border-radius: 32px;
        margin-bottom: 80px;
    }

    .cta-buttons {
        display: flex;
        gap: 16px;
        justify-content: center;
        flex-wrap: wrap;
    }

    .cta-button {
        padding: 12px 32px;
        border-radius: 12px;
        font-weight: 600;
        text-decoration: none;
        transition: all 0.2s ease;
    }

    .cta-button.secondary {
        background: rgba(255, 255, 255, 0.05);
        color: var(--text-primary);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .cta-button.secondary:hover {
        background: rgba(255, 255, 255, 0.08);
    }

    .platform-btn {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 24px;
        padding: 48px 32px;
        min-width: 180px;
        font-family: var(--font-heading);
        font-size: 0.9rem;
    }

    .platform-icon {
        width: 48px;
        height: 48px;
        filter: brightness(0) invert(1);
    }

    .footer {
        padding: 80px 40px;
        color: #444;
        font-size: 0.8rem;
    }

    @media (max-width: 900px) {
        .grid-container,
        .formats-grid {
            grid-template-columns: repeat(2, 1fr);
        }
        .use-cases-grid {
            grid-template-columns: repeat(3, 1fr);
        }
    }

    @media (max-width: 600px) {
        .grid-container,
        .formats-grid,
        .use-cases-grid {
            grid-template-columns: 1fr;
        }
        .hero-title {
            font-size: 3rem;
        }
    }
</style>
