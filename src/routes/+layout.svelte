<script lang="ts">
    import { page } from "$app/stores";

    let { children } = $props();

    const navLinks = [
        { href: "#features", label: "Features" },
        { href: "#formats", label: "Formats" },
        { href: "#download", label: "Download" },
    ];

    let mobileMenuOpen = $state(false);

    function toggleMobileMenu() {
        mobileMenuOpen = !mobileMenuOpen;
    }

    function closeMobileMenu() {
        mobileMenuOpen = false;
    }
</script>

<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link
        rel="preconnect"
        href="https://fonts.gstatic.com"
        crossorigin="anonymous"
    />
    <link
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap"
        rel="stylesheet"
    />
    <style>
        @font-face {
            font-family: "Krona One";
            src: url("/KronaOne-Regular.ttf") format("truetype");
            font-weight: normal;
            font-style: normal;
            font-display: swap;
        }
    </style>
</svelte:head>

<div class="app">
    <nav class="navbar">
        <div class="nav-container">
            <a href="/" class="nav-logo">
                <img src="/capsule.svg" alt="Capsule Logo" class="logo-icon" />
                <span class="logo-text">Capsule</span>
            </a>

            <div class="nav-links-desktop">
                {#each navLinks as link}
                    <a href={link.href} class="nav-link">{link.label}</a>
                {/each}
            </div>

            <div class="nav-actions">
                <a
                    href="https://github.com/kamryn404/Capsule/"
                    class="github-link"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    <img src="/github.svg" alt="GitHub" class="github-icon" />
                </a>
            </div>

            <button
                class="nav-toggle"
                on:click={toggleMobileMenu}
                aria-label="Toggle menu"
            >
                <span class="hamburger" class:open={mobileMenuOpen}></span>
            </button>
        </div>

        {#if mobileMenuOpen}
            <div class="mobile-menu">
                {#each navLinks as link}
                    <a
                        href={link.href}
                        class="mobile-link"
                        on:click={closeMobileMenu}>{link.label}</a
                    >
                {/each}
            </div>
        {/if}
    </nav>

    <main class="main-content">
        {@render children()}
    </main>
</div>

<style>
    :global(:root) {
        --bg-color: #050505;
        --text-primary: #ffffff;
        --text-secondary: #888888;
        --accent-color: #ffffff;
        --font-heading: "Krona One", sans-serif;
        --font-sans:
            "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
            sans-serif;
    }

    :global(html) {
        scroll-behavior: smooth;
    }

    :global(body) {
        margin: 0;
        padding: 0;
        font-family: var(--font-sans);
        background-color: var(--bg-color);
        color: var(--text-primary);
        -webkit-font-smoothing: antialiased;
    }

    .app {
        display: flex;
        flex-direction: column;
        min-height: 100vh;
    }

    .navbar {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        z-index: 1000;
        padding: 20px 0;
        background: linear-gradient(to bottom, rgba(5, 5, 5, 0.8), transparent);
        backdrop-filter: blur(8px);
    }

    .nav-container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 40px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        position: relative;
    }

    .nav-logo {
        text-decoration: none;
        display: flex;
        align-items: center;
        gap: 8px;
    }

    .logo-icon {
        width: 32px;
        height: 32px;
        filter: brightness(0) invert(1);
    }

    .logo-text {
        font-family: var(--font-heading);
        font-size: 1.4rem;
        font-weight: 400;
        color: var(--text-primary);
        letter-spacing: -0.03em;
    }

    .nav-links-desktop {
        display: flex;
        gap: 32px;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
    }

    .nav-link {
        color: var(--text-secondary);
        text-decoration: none;
        font-size: 0.9rem;
        font-weight: 500;
        transition: color 0.2s ease;
    }

    .nav-link:hover {
        color: var(--text-primary);
    }

    .nav-actions {
        display: flex;
        align-items: center;
    }

    .github-icon {
        width: 24px;
        height: 24px;
        filter: brightness(0) invert(1);
        transition: opacity 0.2s ease;
    }

    .github-icon:hover {
        opacity: 0.7;
    }

    .nav-toggle {
        display: none;
        background: none;
        border: none;
        cursor: pointer;
        position: absolute;
        right: 40px;
    }

    .hamburger {
        display: block;
        width: 20px;
        height: 2px;
        background: var(--text-primary);
        position: relative;
    }

    .hamburger::before,
    .hamburger::after {
        content: "";
        position: absolute;
        width: 20px;
        height: 2px;
        background: var(--text-primary);
        left: 0;
        transition: transform 0.2s ease;
    }

    .hamburger::before {
        top: -6px;
    }
    .hamburger::after {
        top: 6px;
    }

    .hamburger.open {
        background: transparent;
    }
    .hamburger.open::before {
        transform: translateY(6px) rotate(45deg);
    }
    .hamburger.open::after {
        transform: translateY(-6px) rotate(-45deg);
    }

    .mobile-menu {
        position: fixed;
        top: 70px;
        left: 0;
        right: 0;
        background: var(--bg-color);
        padding: 20px 40px;
        display: flex;
        flex-direction: column;
        gap: 20px;
        border-bottom: 1px solid #222;
    }

    .mobile-link {
        color: var(--text-primary);
        text-decoration: none;
        font-size: 1.2rem;
    }

    .main-content {
        flex: 1;
    }

    @media (max-width: 768px) {
        .nav-links-desktop,
        .nav-actions {
            display: none;
        }
        .nav-toggle {
            display: block;
        }
        .nav-container {
            justify-content: space-between;
        }
    }
</style>
