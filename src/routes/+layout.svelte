<svelte:head>
    <meta
        name="description"
        content="Ellatech Energy Services Ltd provides electrical, instrumentation, procurement, construction, commissioning, calibration, pressure testing, and industrial support services."
    />
    <meta name="theme-color" content="#0f4c81" />
</svelte:head>

<script lang="ts">
    const navItems = [
        { label: "Home", href: "#home" },
        { label: "About", href: "#about" },
        { label: "Services", href: "#services" },
        { label: "Values", href: "#values" },
        { label: "Contact", href: "#contact" }
    ];

    const services = [
        "Electrical / Instrument Works",
        "Instrument Calibration",
        "Electrical / Instrument Inspection",
        "Metering and Proving Systems",
        "Fire and Gas",
        "HVAC",
        "Pressure Testing",
        "Procurement",
        "Training, Consultancy and Manpower Supply"
    ];
</script>

<div class="site-shell">
    <div class="page-glow page-glow-left"></div>
    <div class="page-glow page-glow-right"></div>

    <header class="site-header">
        <div class="container shell-row topbar">
            <p>Electrical and instrumentation support for oil, gas and industrial operations</p>
            <a href="tel:+234084302488">+234 084302488</a>
        </div>

        <div class="container shell-row navbar">
            <a class="brand" href="#home" aria-label="Ellatech Energy Services Ltd home">
                <img src="/assets/images/logo.jpeg" alt="Ellatech Energy Services Ltd" />
            </a>

            <nav class="site-nav" aria-label="Primary">
                {#each navItems as item}
                    <a href={item.href}>{item.label}</a>
                {/each}
            </nav>

            <div class="header-actions">
                <a
                    class="header-webmail"
                    href="https://host.mcreal56.net:2096/"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    Webmail
                </a>
                <a class="header-cta" href="#contact">Request Support</a>
            </div>
        </div>
    </header>

    <main>
        <slot />
    </main>

    <footer class="site-footer" id="contact">
        <div class="container footer-grid">
            <div>
                <a class="footer-brand" href="#home">
                    <img src="/assets/images/logo.jpeg" alt="Ellatech Energy Services Ltd" />
                </a>
                <p class="footer-copy">
                    Viable indigenous engineering support across procurement,
                    construction, commissioning, calibration and maintenance.
                </p>
            </div>

            <div>
                <h2>Quick Links</h2>
                <div class="footer-links">
                    {#each navItems as item}
                        <a href={item.href}>{item.label}</a>
                    {/each}
                </div>
            </div>

            <div>
                <h2>Core Services</h2>
                <ul class="footer-services">
                    {#each services as service}
                        <li>{service}</li>
                    {/each}
                </ul>
            </div>

            <div>
                <h2>Contact</h2>
                <div class="contact-stack">
                    <p>
                        305 Port Harcourt/Aba Expressway, Opposite Trust Fund,
                        after Rumuokwurushi junction, Port Harcourt, Rivers
                        State, Nigeria.
                    </p>
                    <a href="tel:+2340804302488">+234 0804302488</a>
                    <a href="mailto:info@ellatechg.com">info@ellatechg.com</a>
                </div>
            </div>
        </div>

        <div class="container footer-bottom">
            <p>Copyright © 2026 Ellatech Energy Services Ltd. All rights reserved.</p>
            <a href="#home">Back to top</a>
        </div>
    </footer>
</div>

<style>
    :global(html) {
        scroll-behavior: smooth;
    }

    :global(body) {
        margin: 0;
        color: #12304b;
        font-family: "Manrope", "Segoe UI", sans-serif;
        background:
            radial-gradient(circle at top left, rgba(100, 195, 255, 0.28), transparent 28%),
            linear-gradient(180deg, #f5fbff 0%, #eef6fb 54%, #f7fbfe 100%);
    }

    :global(*) {
        box-sizing: border-box;
    }

    :global(img) {
        display: block;
        max-width: 100%;
    }

    :global(a) {
        color: inherit;
        text-decoration: none;
    }

    .site-shell {
        position: relative;
        overflow: clip;
    }

    .page-glow {
        position: fixed;
        z-index: -1;
        width: 28rem;
        height: 28rem;
        border-radius: 999px;
        filter: blur(70px);
        opacity: 0.32;
        pointer-events: none;
    }

    .page-glow-left {
        top: -7rem;
        left: -9rem;
        background: #5bbcff;
    }

    .page-glow-right {
        top: 18rem;
        right: -10rem;
        background: #0f4c81;
    }

    .container {
        width: min(1180px, calc(100% - 2rem));
        margin: 0 auto;
    }

    .shell-row {
        display: flex;
        align-items: center;
        justify-content: space-between;
        gap: 1rem;
    }

    .site-header {
        position: sticky;
        top: 0;
        z-index: 20;
        backdrop-filter: blur(20px);
        background: rgba(247, 251, 254, 0.72);
        border-bottom: 1px solid rgba(15, 76, 129, 0.08);
    }

    .topbar {
        padding: 0.8rem 0;
        color: #48657f;
        font-size: 0.85rem;
    }

    .topbar p {
        margin: 0;
    }

    .topbar a {
        font-weight: 700;
        color: #0f4c81;
    }

    .navbar {
        padding: 1rem 0 1.1rem;
    }

    .brand {
        flex: 0 0 auto;
    }

    .brand img,
    .footer-brand img {
        width: min(280px, 62vw);
        max-height: 4.75rem;
        height: auto;
        object-fit: contain;
    }

    .site-nav {
        display: flex;
        align-items: center;
        gap: 0.4rem;
        padding: 0.35rem;
        border: 1px solid rgba(15, 76, 129, 0.08);
        border-radius: 999px;
        background: rgba(255, 255, 255, 0.82);
        box-shadow: 0 14px 34px rgba(15, 76, 129, 0.08);
    }

    .site-nav a,
    .header-webmail,
    .header-cta,
    .footer-bottom a {
        transition:
            transform 0.2s ease,
            background 0.2s ease,
            color 0.2s ease,
            border-color 0.2s ease;
    }

    .site-nav a {
        padding: 0.7rem 1rem;
        border-radius: 999px;
        color: #34526d;
        font-weight: 700;
        font-size: 0.95rem;
    }

    .site-nav a:hover {
        background: rgba(15, 76, 129, 0.08);
        color: #0f4c81;
        transform: translateY(-1px);
    }

    .header-actions {
        display: flex;
        align-items: center;
        gap: 0.75rem;
    }

    .header-webmail,
    .header-cta {
        padding: 0.9rem 1.25rem;
        border-radius: 999px;
        font-weight: 800;
    }

    .header-webmail {
        border: 1px solid rgba(15, 76, 129, 0.14);
        background: rgba(255, 255, 255, 0.9);
        color: #0f4c81;
        box-shadow: 0 14px 30px rgba(15, 76, 129, 0.08);
    }

    .header-cta {
        background: linear-gradient(135deg, #0f4c81, #2aa1db);
        color: #fff;
        box-shadow: 0 14px 30px rgba(15, 76, 129, 0.18);
    }

    .header-webmail:hover,
    .header-cta:hover,
    .footer-bottom a:hover {
        transform: translateY(-2px);
    }

    .site-footer {
        margin-top: 5rem;
        padding: 4rem 0 1.5rem;
        color: rgba(255, 255, 255, 0.88);
        background:
            radial-gradient(circle at top left, rgba(43, 161, 219, 0.2), transparent 22%),
            linear-gradient(180deg, #123552 0%, #0a2439 100%);
    }

    .footer-grid {
        display: grid;
        grid-template-columns: 1.3fr 0.9fr 1fr 1.1fr;
        gap: 2rem;
    }

    .site-footer h2 {
        margin: 0 0 1rem;
        font-family: "Space Grotesk", "Segoe UI", sans-serif;
        font-size: 1.1rem;
        color: #fff;
    }

    .footer-copy,
    .contact-stack p,
    .footer-services li,
    .footer-links a {
        color: rgba(255, 255, 255, 0.78);
        line-height: 1.7;
    }

    .footer-links,
    .contact-stack {
        display: grid;
        gap: 0.65rem;
    }

    .footer-links a:hover,
    .contact-stack a:hover {
        color: #7fd4ff;
    }

    .footer-services {
        display: grid;
        gap: 0.6rem;
        padding: 0;
        margin: 0;
        list-style: none;
    }

    .footer-bottom {
        display: flex;
        align-items: center;
        justify-content: space-between;
        gap: 1rem;
        margin-top: 2.4rem;
        padding-top: 1.25rem;
        border-top: 1px solid rgba(255, 255, 255, 0.12);
        font-size: 0.92rem;
    }

    .footer-bottom p {
        margin: 0;
    }

    .footer-bottom a {
        padding: 0.75rem 1rem;
        border: 1px solid rgba(255, 255, 255, 0.16);
        border-radius: 999px;
    }

    @media (max-width: 1040px) {
        .navbar {
            flex-wrap: wrap;
        }

        .site-nav {
            order: 3;
            width: 100%;
            justify-content: center;
            flex-wrap: wrap;
            border-radius: 1.25rem;
        }

        .header-actions {
            width: 100%;
            justify-content: flex-end;
        }

        .footer-grid {
            grid-template-columns: repeat(2, minmax(0, 1fr));
        }
    }

    @media (max-width: 720px) {
        .container {
            width: min(100% - 1.25rem, 1180px);
        }

        .topbar,
        .footer-bottom {
            flex-direction: column;
            align-items: flex-start;
        }

        .topbar {
            padding: 0.7rem 0;
        }

        .navbar {
            padding: 0.8rem 0 1rem;
        }

        .site-nav a {
            width: 100%;
            text-align: center;
        }

        .header-actions {
            width: 100%;
            flex-direction: column;
        }

        .header-webmail,
        .header-cta {
            width: 100%;
            text-align: center;
        }

        .footer-grid {
            grid-template-columns: 1fr;
        }
    }
</style>
