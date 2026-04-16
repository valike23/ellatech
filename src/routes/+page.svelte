<script lang="ts">
    const serviceCards = [
        {
            title: "Electrical / Instrument Works",
            copy: "Field installation, hook-up, revamp work and commissioning support for plant and facility operations."
        },
        {
            title: "Instrument Calibration",
            copy: "Calibration and verification support for critical instruments to keep operations stable, safe and compliant."
        },
        {
            title: "Electrical / Instrument Inspection",
            copy: "Inspection, troubleshooting and reliability support for installed electrical and instrumentation systems."
        },
        {
            title: "Metering and Proving Systems",
            copy: "Metering, proving and liquid handling support for industrial process and transfer environments."
        },
        {
            title: "Fire and Gas",
            copy: "Support for fire and gas systems that help protect people, assets and process continuity."
        },
        {
            title: "HVAC",
            copy: "Mechanical and facility support that helps maintain workable, controlled operating conditions."
        },
        {
            title: "Pressure Testing",
            copy: "Pressure testing of vessels and related systems, including PRV calibration support."
        },
        {
            title: "Procurement",
            copy: "Responsive sourcing and procurement assistance for project delivery, maintenance and shutdown needs."
        },
        {
            title: "Training, Consultancy and Manpower Supply",
            copy: "Experienced technical support, advisory input and labour supply tailored to client requirements."
        }
    ];

    const values = [
        "We serve willingly in all work locations and conditions.",
        "We care for the safety, security, development and well-being of our employees while paying close attention to our working environment.",
        "We empower our employees to succeed in a culture based on trust, respect, loyalty and commitment.",
        "We perform with a relentless commitment to exceeding expectations.",
        "We do the right thing always for our customers, employees and those we serve."
    ];

    const highlights = [
        "Engineering, Procurement, Construction and Commissioning support",
        "Electrical and instrumentation activities across industrial sectors",
        "Minor fabrication, pipework installation and labour supply",
        "Cost-effective solutions tailored to client budgets"
    ];

    const gallery = [
        {
            image: "/assets/images/slider/oilring1.jpeg",
            title: "Industrial Electrical Support"
        },
        {
            image: "/assets/images/about/about-3.jpg",
            title: "Calibration and Plant Access"
        },
        {
            image: "/assets/images/slider/team.jpeg",
            title: "Field Teams and Commissioning"
        }
    ];
</script>

<svelte:head>
    <title>Ellatech Energy Services Ltd</title>
</svelte:head>

<section class="hero" id="home">
    <div class="container hero-grid">
        <div class="hero-copy">
            <span class="eyebrow">Ellatech Energy Services Ltd</span>
            <h1>Modern industrial support built on electrical and instrumentation expertise.</h1>
            <p class="lead">
                Ellatech is a viable indigenous company delivering engineering,
                procurement, construction and commissioning support with a focus
                on electrical and instrumentation activities for oil, gas and
                allied industrial sectors.
            </p>

            <div class="cta-row">
                <a class="primary-btn" href="#services">Explore Services</a>
                <a class="secondary-btn" href="#about">About Ellatech</a>
            </div>

            <div class="hero-pills">
                {#each highlights as item}
                    <span>{item}</span>
                {/each}
            </div>
        </div>

        <div class="hero-visual">
            <div class="visual-card visual-main">
                <img
                    src="/assets/images/slider/oilring1.jpeg"
                    alt="Engineer working on an industrial control panel"
                />
            </div>

            <div class="visual-card visual-note">
                <p class="note-label">What we handle</p>
                <h2>Calibration, hook-ups, proving, pressure testing and pipework installation.</h2>
            </div>

            <div class="visual-card visual-stat">
                <span>Since 2013</span>
                <p>Supporting safe, cost-conscious delivery for industrial clients.</p>
            </div>
        </div>
    </div>
</section>

<section class="summary-band">
    <div class="container band-grid">
        <article>
            <span>Mission</span>
            <p>
                To provide quality electrical and instrumentation services
                through seasoned engineering that helps clients achieve
                cost-effective production tailored to budget.
            </p>
        </article>
        <article>
            <span>Coverage</span>
            <p>
                We work across oil and gas, petrochemical and allied industries
                with flexible support for plant, field and facility conditions.
            </p>
        </article>
        <article>
            <span>Approach</span>
            <p>
                Practical engineering, clear execution and dependable manpower
                support focused on safe delivery and operational continuity.
            </p>
        </article>
    </div>
</section>

<section class="section-block about" id="about">
    <div class="container two-column">
        <div class="section-intro">
            <span class="eyebrow">About Us</span>
            <h2>Built to support complex plant operations with dependable field execution.</h2>
            <p>
                We specialize in major aspects of electrical and instrumentation
                activities including instrument calibration, E and I
                installation, hook-ups, revamp work, liquid handling, metering
                and proving services, pressure testing of vessels, PRV
                calibration, minor fabrication and the installation of pipework.
            </p>
            <p>
                Our goal is simple: give clients practical, production-minded
                support that improves delivery quality without losing sight of
                cost, safety or schedule.
            </p>
        </div>

        <div class="about-stack">
            <img
                class="about-image"
                src="/assets/images/about/about-3.jpg"
                alt="Ellatech team member working in an industrial facility"
            />

            <div class="about-panel">
                <h3>Operational Base</h3>
                <p>
                    305 Port Harcourt/Aba Expressway, Opposite Trust Fund, after
                    Rumuokwurushi junction, Port Harcourt, Rivers State,
                    Nigeria.
                </p>
                <div class="link-pair">
                    <a href="tel:+2340804302488">+234 0804302488</a>
                    <a href="mailto:info@ellatechg.com">info@ellatechg.com</a>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="section-block services" id="services">
    <div class="container">
        <div class="section-heading">
            <span class="eyebrow">Our Services</span>
            <h2>Capabilities shaped by real operational needs.</h2>
            <p>
                From field installation to inspection, testing and manpower
                supply, Ellatech supports the work that keeps industrial assets
                moving.
            </p>
        </div>

        <div class="service-grid">
            {#each serviceCards as service}
                <article class="service-card">
                    <div class="service-icon"></div>
                    <h3>{service.title}</h3>
                    <p>{service.copy}</p>
                </article>
            {/each}
        </div>
    </div>
</section>

<section class="section-block values" id="values">
    <div class="container values-grid">
        <div class="values-copy">
            <span class="eyebrow">Our Core Values</span>
            <h2>We are Ellatech when service, safety and integrity show up together.</h2>
            <p>
                The old site spoke plainly about who Ellatech is. We’ve kept
                that spirit here and turned it into a clearer statement of how
                the company works with clients, teams and communities.
            </p>
            <div class="mission-quote">
                <span>Our Mission</span>
                <p>
                    "Provide quality electrical and instrumentation services
                    through seasoned engineering to deliver cost-effective
                    production properly tailored to client budgets."
                </p>
            </div>
        </div>

        <div class="value-list">
            {#each values as value, index}
                <article class="value-card">
                    <span>{String(index + 1).padStart(2, "0")}</span>
                    <p>{value}</p>
                </article>
            {/each}
        </div>
    </div>
</section>

<section class="section-block gallery">
    <div class="container">
        <div class="section-heading">
            <span class="eyebrow">Field Gallery</span>
            <h2>A cleaner view of Ellatech’s working environment.</h2>
            <p>
                The original site relied on dense copy and small images. This
                updated layout gives the visual story more space while keeping
                the industrial focus front and center.
            </p>
        </div>

        <div class="gallery-grid">
            {#each gallery as item}
                <figure class="gallery-card">
                    <img src={item.image} alt={item.title} />
                    <figcaption>{item.title}</figcaption>
                </figure>
            {/each}
        </div>
    </div>
</section>

<section class="cta-strip">
    <div class="container cta-shell">
        <div>
            <span class="eyebrow">Ready to Engage?</span>
            <h2>Bring Ellatech into your next project, shutdown or maintenance cycle.</h2>
        </div>

        <div class="cta-actions">
            <a class="primary-btn" href="mailto:info@ellatechg.com">Email Ellatech</a>
            <a class="secondary-btn dark" href="tel:+2340804302488">Call Now</a>
        </div>
    </div>
</section>

<style>
    .container {
        width: min(1180px, calc(100% - 2rem));
        margin: 0 auto;
    }

    .hero {
        padding: 4.5rem 0 2.5rem;
    }

    .hero-grid,
    .two-column,
    .values-grid,
    .cta-shell {
        display: grid;
        gap: 2rem;
        align-items: center;
    }

    .hero-grid {
        grid-template-columns: minmax(0, 0.55fr) minmax(0, 1.45fr);
    }

    .eyebrow {
        display: inline-flex;
        align-items: center;
        gap: 0.5rem;
        padding: 0.45rem 0.8rem;
        border-radius: 999px;
        background: rgba(15, 76, 129, 0.08);
        color: #0f4c81;
        font-size: 0.82rem;
        font-weight: 800;
        letter-spacing: 0.08em;
        text-transform: uppercase;
    }

    .hero-copy h1,
    .section-heading h2,
    .section-intro h2,
    .values-copy h2,
    .cta-shell h2,
    .visual-note h2 {
        margin: 0;
        font-family: "Space Grotesk", "Segoe UI", sans-serif;
        line-height: 1.02;
        color: #12304b;
    }

    .hero-copy h1 {
        margin-top: 1.15rem;
        font-size: clamp(1.5rem, 2.5vw, 2.65rem);
        max-width: 9ch;
    }

    .lead,
    .section-heading p,
    .section-intro p,
    .values-copy p,
    .service-card p,
    .mission-quote p,
    .gallery-card figcaption {
        color: #4e6a82;
        line-height: 1.8;
    }

    .lead {
        margin: 1.3rem 0 0;
        max-width: 62ch;
        font-size: 1.05rem;
    }

    .cta-row,
    .cta-actions,
    .link-pair {
        display: flex;
        flex-wrap: wrap;
        gap: 0.9rem;
        margin-top: 1.7rem;
    }

    .primary-btn,
    .secondary-btn {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        min-height: 3.35rem;
        padding: 0.95rem 1.35rem;
        border-radius: 999px;
        font-weight: 800;
        transition:
            transform 0.2s ease,
            box-shadow 0.2s ease,
            border-color 0.2s ease,
            background 0.2s ease;
    }

    .primary-btn {
        color: #fff;
        background: linear-gradient(135deg, #0f4c81, #2aa1db);
        box-shadow: 0 18px 32px rgba(15, 76, 129, 0.2);
    }

    .secondary-btn {
        border: 1px solid rgba(15, 76, 129, 0.14);
        background: rgba(255, 255, 255, 0.9);
        color: #0f4c81;
    }

    .secondary-btn.dark {
        color: #fff;
        border-color: rgba(255, 255, 255, 0.22);
        background: rgba(255, 255, 255, 0.08);
    }

    .primary-btn:hover,
    .secondary-btn:hover {
        transform: translateY(-2px);
    }

    .hero-pills {
        display: flex;
        flex-wrap: wrap;
        gap: 0.75rem;
        margin-top: 1.8rem;
    }

    .hero-pills span,
    .service-icon {
        border: 1px solid rgba(15, 76, 129, 0.08);
        background: rgba(255, 255, 255, 0.72);
        box-shadow: 0 18px 38px rgba(15, 76, 129, 0.08);
    }

    .hero-pills span {
        padding: 0.75rem 0.95rem;
        border-radius: 1rem;
        color: #36546d;
        font-weight: 700;
    }

    .hero-visual {
        position: relative;
        min-height: 75vh;
    }

    .visual-card,
    .service-card,
    .about-panel,
    .value-card,
    .gallery-card,
    .summary-band article,
    .mission-quote {
        border: 1px solid rgba(15, 76, 129, 0.08);
        border-radius: 1.6rem;
        background: rgba(255, 255, 255, 0.78);
        box-shadow: 0 22px 54px rgba(15, 76, 129, 0.1);
        backdrop-filter: blur(10px);
    }

    .visual-main {
        position: absolute;
        inset: 0 0 5.5rem 0;
        overflow: hidden;
    }

    .visual-main img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
    }

    .visual-note {
        position: absolute;
        right: 0;
        bottom: 6.7rem;
        width: min(22rem, 46%);
        padding: 1.4rem;
    }

    .visual-note h2 {
        font-size: 1.45rem;
    }

    .visual-stat {
        position: absolute;
        left: 1.4rem;
        bottom: 0;
        width: min(19rem, 36%);
        padding: 1.25rem 1.35rem;
        background: linear-gradient(135deg, #123d65, #2aa1db);
        color: #fff;
    }

    .visual-stat span,
    .note-label,
    .summary-band span,
    .mission-quote span {
        display: inline-block;
        font-size: 0.78rem;
        font-weight: 800;
        letter-spacing: 0.08em;
        text-transform: uppercase;
    }

    .visual-stat p,
    .summary-band p,
    .about-panel p {
        margin: 0.65rem 0 0;
        line-height: 1.75;
    }

    .summary-band {
        padding: 1.2rem 0 0.5rem;
    }

    .band-grid {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 1rem;
    }

    .summary-band article {
        padding: 1.4rem;
    }

    .summary-band span,
    .mission-quote span {
        color: #0f4c81;
    }

    .section-block {
        padding: 4.25rem 0 0;
    }

    .two-column,
    .values-grid,
    .cta-shell {
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .section-intro,
    .values-copy {
        display: grid;
        gap: 1rem;
    }

    .section-intro h2,
    .section-heading h2,
    .values-copy h2,
    .cta-shell h2 {
        font-size: clamp(2rem, 3vw, 3.2rem);
    }

    .about-stack {
        display: grid;
        gap: 1.2rem;
    }

    .about-image,
    .gallery-card img {
        width: 100%;
        border-radius: 1.6rem;
        object-fit: cover;
    }

    .about-image {
        min-height: 28rem;
    }

    .about-panel {
        padding: 1.5rem;
    }

    .about-panel h3,
    .service-card h3 {
        margin: 0;
        font-family: "Space Grotesk", "Segoe UI", sans-serif;
        color: #12304b;
    }

    .section-heading {
        max-width: 46rem;
        display: grid;
        gap: 1rem;
        margin-bottom: 1.8rem;
    }

    .service-grid,
    .gallery-grid {
        display: grid;
        gap: 1rem;
    }

    .service-grid {
        grid-template-columns: repeat(3, minmax(0, 1fr));
    }

    .service-card {
        display: grid;
        gap: 1rem;
        padding: 1.4rem;
    }

    .service-icon {
        width: 3.25rem;
        height: 3.25rem;
        border-radius: 1rem;
        background:
            radial-gradient(circle at top left, rgba(43, 161, 219, 0.85), rgba(15, 76, 129, 0.9)),
            rgba(255, 255, 255, 0.72);
    }

    .service-card p {
        margin: 0;
    }

    .values-grid {
        align-items: start;
    }

    .mission-quote {
        padding: 1.35rem;
        margin-top: 0.4rem;
    }

    .value-list {
        display: grid;
        gap: 1rem;
    }

    .value-card {
        display: grid;
        grid-template-columns: auto 1fr;
        gap: 1rem;
        align-items: start;
        padding: 1.25rem 1.35rem;
    }

    .value-card span {
        width: 2.75rem;
        height: 2.75rem;
        display: inline-flex;
        align-items: center;
        justify-content: center;
        border-radius: 999px;
        background: rgba(15, 76, 129, 0.1);
        color: #0f4c81;
        font-weight: 900;
    }

    .value-card p {
        margin: 0;
        color: #415f78;
        line-height: 1.8;
    }

    .gallery-grid {
        grid-template-columns: 1.2fr 0.8fr 0.95fr;
    }

    .gallery-card {
        overflow: hidden;
    }

    .gallery-card img {
        height: 21rem;
    }

    .gallery-card figcaption {
        padding: 1rem 1.15rem 1.2rem;
        font-weight: 800;
        color: #12304b;
    }

    .cta-strip {
        padding: 4.5rem 0 0;
    }

    .cta-shell {
        padding: 2rem;
        border-radius: 2rem;
        background:
            radial-gradient(circle at top right, rgba(127, 212, 255, 0.24), transparent 25%),
            linear-gradient(135deg, #123d65, #0d2d49 52%, #0a2439 100%);
        color: #fff;
    }

    .cta-shell h2 {
        max-width: 12ch;
        color: #fff;
    }

    @media (max-width: 1040px) {
        .hero-grid,
        .two-column,
        .values-grid,
        .cta-shell,
        .service-grid,
        .gallery-grid,
        .band-grid {
            grid-template-columns: repeat(2, minmax(0, 1fr));
        }

        .hero-visual {
            min-height: 42rem;
        }

        .gallery-card:first-child {
            grid-column: 1 / -1;
        }
    }

    @media (max-width: 720px) {
        .container {
            width: min(100% - 1.25rem, 1180px);
        }

        .hero {
            padding-top: 2rem;
        }

        .hero-grid,
        .two-column,
        .values-grid,
        .cta-shell,
        .service-grid,
        .gallery-grid,
        .band-grid {
            grid-template-columns: 1fr;
        }

        .hero-copy h1 {
            max-width: 100%;
            font-size: clamp(1.9rem, 9vw, 2.6rem);
        }

        .hero-visual {
            min-height: 34rem;
        }

        .visual-main {
            inset: 0 0 6.2rem;
        }

        .visual-note,
        .visual-stat {
            width: calc(100% - 1rem);
        }

        .visual-note {
            right: 0.5rem;
            bottom: 7.2rem;
        }

        .visual-stat {
            left: 0.5rem;
        }

        .about-image,
        .gallery-card img {
            min-height: auto;
            height: 18rem;
        }

        .cta-shell {
            padding: 1.5rem;
        }

        .cta-shell h2 {
            max-width: none;
        }
    }
</style>
