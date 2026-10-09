<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gesundheit & Vitalität | Offizielles deutsches Prüfportal 2026</title>
    <style>
        /* Global & Reset Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: #f8fafc;
            color: #1e293b;
            line-height: 1.6;
        }

        /* Top Disclosure Banner */
        .top-bar {
            background-color: #0f172a;
            color: #f8fafc;
            text-align: center;
            padding: 8px 12px;
            font-size: 12px;
            border-bottom: 3px solid #dd0000;
        }

        /* Navigation Bar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #ffffff;
            padding: 15px 5%;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }

        .logo {
            font-size: 24px;
            font-weight: 800;
            color: #0f172a;
        }

        .logo span {
            color: #dd0000;
        }

        .navbar ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .navbar a {
            text-decoration: none;
            color: #475569;
            font-weight: 600;
            font-size: 14px;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #0f172a, #1e293b);
            color: #ffffff;
            padding: 50px 20px;
            text-align: center;
        }

        .hero .tag {
            background-color: #dd0000;
            color: #fff;
            padding: 4px 12px;
            border-radius: 4px;
            font-size: 11px;
            text-transform: uppercase;
            font-weight: bold;
        }

        .hero h1 {
            font-size: 28px;
            margin: 15px 0 10px 0;
        }

        .hero p {
            font-size: 15px;
            color: #94a3b8;
            max-width: 650px;
            margin: 0 auto;
        }

        /* Main Container & Product Cards */
        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .container h2 {
            text-align: center;
            font-size: 26px;
            color: #0f172a;
        }

        .section-subtitle {
            text-align: center;
            color: #64748b;
            margin-bottom: 30px;
            font-size: 14px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(290px, 1fr));
            gap: 25px;
        }

        .product-card {
            background: #ffffff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            border: 1px solid #e2e8f0;
        }

        .card-header {
            position: relative;
        }

        .card-header img {
            width: 100%;
            height: auto;
            display: block;
        }

        .badge {
            position: absolute;
            top: 12px;
            left: 12px;
            color: #fff;
            padding: 4px 10px;
            font-size: 11px;
            font-weight: bold;
            border-radius: 4px;
        }

        .badge.red { background-color: #dc2626; }
        .badge.green { background-color: #16a34a; }
        .badge.blue { background-color: #2563eb; }

        .card-body {
            padding: 20px;
        }

        .card-body h3 {
            font-size: 19px;
            margin-bottom: 5px;
            color: #0f172a;
        }

        .category {
            font-size: 12px;
            color: #64748b;
            margin-bottom: 10px;
        }

        .stars {
            color: #f59e0b;
            font-weight: bold;
            font-size: 14px;
            margin-bottom: 15px;
        }

        .stars span {
            color: #64748b;
            font-weight: normal;
            font-size: 12px;
        }

        .benefits {
            list-style: none;
            font-size: 13px;
            color: #334155;
            margin-bottom: 20px;
        }

        .benefits li {
            margin-bottom: 8px;
        }

        .price-box {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 15px;
        }

        .old-price {
            text-decoration: line-through;
            color: #94a3b8;
            font-size: 15px;
        }

        .new-price {
            font-size: 22px;
            font-weight: bold;
            color: #dc2626;
        }

        .discount {
            background-color: #fef2f2;
            color: #dc2626;
            padding: 2px 8px;
            font-size: 12px;
            font-weight: bold;
            border-radius: 4px;
            border: 1px solid #fecaca;
        }

        .cta-button {
            display: block;
            text-align: center;
            background-color: #16a34a;
            color: #ffffff;
            padding: 12px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: bold;
            font-size: 14px;
            transition: background 0.3s;
        }

        .cta-button:hover {
            background-color: #15803d;
        }

        /* Trust Badges */
        .trust-section {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .trust-box {
            background: #ffffff;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 2px 8px rgba(0,0,0,0.04);
            border: 1px solid #e2e8f0;
        }

        .trust-box h4 {
            color: #0f172a;
            margin-bottom: 8px;
        }

        .trust-box p {
            font-size: 13px;
            color: #64748b;
        }

        /* Legal Section (German Impressum) */
        .legal-section {
            background: #f1f5f9;
            padding: 30px 5%;
            font-size: 13px;
            margin-top: 40px;
            border-top: 1px solid #e2e8f0;
        }

        .legal-section h3 {
            margin-bottom: 10px;
            color: #0f172a;
        }

        footer {
            background-color: #0f172a;
            color: #94a3b8;
            padding: 25px 20px;
            text-align: center;
            font-size: 12px;
        }

        .disclaimer {
            font-size: 11px;
            margin: 10px 0;
            color: #64748b;
        }

        .footer-links a {
            color: #cbd5e1;
            text-decoration: none;
            margin: 0 5px;
        }
    </style>
</head>
<body>

    <!-- German EU Disclosure Banner -->
    <div class="top-bar">
        <span>🇩🇪 Offizielles Prüfportal für Deutschland | Transparenz-Hinweis: Unabhängige Produktempfehlungen</span>
    </div>

    <!-- Header Navigation -->
    <header class="navbar">
        <div class="logo">Gesundheits<span>DE</span></div>
        <nav>
            <ul>
                <li><a href="#home">Startseite</a></li>
                <li><a href="#empfehlungen">Top-Empfehlungen</a></li>
                <li><a href="#impressum">Impressum</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <span class="tag">Geprüfte Qualität in Deutschland</span>
            <h1>Natürliche Gesundheitsprodukte im Unabhängigen Vergleich</h1>
            <p>Ehrliche Tests, klinisch geprüfte Inhaltsstoffe und exklusive Angebote mit Lieferung auf Nachnahme.</p>
        </div>
    </section>

    <!-- Product Offers Section -->
    <section id="empfehlungen" class="container">
        <h2>Die beliebtesten Gesundheitsprodukte in Deutschland (2026)</h2>
        <p class="section-subtitle">Von Anwendern in Deutschland am besten bewertet.</p>

        <div class="product-grid">

            <!-- Offer 1: Weight Loss -->
            <div class="product-card">
                <div class="card-header">
                    <span class="badge red">Testsieger 2026</span>
                    <img src="https://via.placeholder.com/300x220?text=Keto+Complex+DE" alt="Keto Tropfen">
                </div>
                <div class="card-body">
                    <h3>Keto Slimming Tropfen Pro</h3>
                    <p class="category">Kategorie: Gewichtsmanagement & Stoffwechsel</p>
                    <div class="stars">★★★★★ <span>(4.9/5 - 2.840 Bewertungen)</span></div>
                    
                    <ul class="benefits">
                        <li>✔ Aktiviert den natürlichen Fettstoffwechsel</li>
                        <li>✔ Ohne mühsames Kalorienzählen</li>
                        <li>✔ 100% Natürliche Inhaltsstoffe aus der EU</li>
                    </ul>

                    <div class="price-box">
                        <span class="old-price">98 €</span>
                        <span class="new-price">49 €</span>
                        <span class="discount">-50% Rabatt</span>
                    </div>

                    <!-- Replace with Dr.cash Affiliate Link -->
                    <a href="YOUR_DR_CASH_LINK_HERE" target="_blank" class="cta-button">Jetzt 50% Rabatt Sichern*</a>
                </div>
            </div>

            <!-- Offer 2: Joint Care -->
            <div class="product-card">
                <div class="card-header">
                    <span class="badge green">Bestseller in Deutschland</span>
                    <img src="https://via.placeholder.com/300x220?text=Gelenk+Balsam+DE" alt="Gelenk Gel">
                </div>
                <div class="card-body">
                    <h3>Gelenk-Aktiv Balsam Premium</h3>
                    <p class="category">Kategorie: Gelenke & Beweglichkeit</p>
                    <div class="stars">★★★★☆ <span>(4.8/5 - 1.950 Bewertungen)</span></div>
                    
                    <ul class="benefits">
                        <li>✔ Schnelle Beruhigung bei Bewegungseinschränkungen</li>
                        <li>✔ Zieht schnell ein, ohne zu kleben</li>
                        <li>✔ Dermatologisch in Deutschland getestet</li>
                    </ul>

                    <div class="price-box">
                        <span class="old-price">78 €</span>
                        <span class="new-price">39 €</span>
                        <span class="discount">-50% Rabatt</span>
                    </div>

                    <!-- Replace with Dr.cash Affiliate Link -->
                    <a href="YOUR_DR_CASH_LINK_HERE" target="_blank" class="cta-button">Jetzt 50% Rabatt Sichern*</a>
                </div>
            </div>

            <!-- Offer 3: Anti-Aging -->
            <div class="product-card">
                <div class="card-header">
                    <span class="badge blue">Neuerscheinung</span>
                    <img src="https://via.placeholder.com/300x220?text=Hyaluron+Serum+DE" alt="Hyaluron Serum">
                </div>
                <div class="card-body">
                    <h3>Hyaluron Anti-Falten Serum</h3>
                    <p class="category">Kategorie: Hautpflege & Anti-Aging</p>
                    <div class="stars">★★★★★ <span>(4.9/5 - 3.120 Bewertungen)</span></div>
                    
                    <ul class="benefits">
                        <li>✔ Minderung sichtbarer Fältchen im Gesicht</li>
                        <li>✔ Tiefenwirksame Feuchtigkeitszufuhr</li>
                        <li>✔ Für empfindliche Haut geeignet</li>
                    </ul>

                    <div class="price-box">
                        <span class="old-price">88 €</span>
                        <span class="new-price">44 €</span>
                        <span class="discount">-50% Rabatt</span>
                    </div>

                    <!-- Replace with Dr.cash Affiliate Link -->
                    <a href="YOUR_DR_CASH_LINK_HERE" target="_blank" class="cta-button">Jetzt 50% Rabatt Sichern*</a>
                </div>
            </div>

        </div>
    </section>

    <!-- Trust Features -->
    <section class="trust-section">
        <div class="trust-box">
            <h4>🚚 Schnelle Lieferung</h4>
            <p>Lieferung innerhalb von 2-3 Werktagen per DHL / Hermes in ganz Deutschland.</p>
        </div>
        <div class="trust-box">
            <h4>💶 Bezahlung per Nachnahme</h4>
            <p>Keine Kreditkarte erforderlich. Zahlen Sie erst bequem an der Haustür.</p>
        </div>
        <div class="trust-box">
            <h4>🌿 Premium Qualität</h4>
            <p>Hergestellt nach strengen deutschen und EU-Qualitätsstandards.</p>
        </div>
    </section>

    <!-- German Legal Impressum (Mandatory for Germany) -->
    <section id="impressum" class="legal-section">
        <div class="container">
            <h3>Impressum & Rechtliche Hinweise</h3>
            <p><strong>Angaben gemäß § 5 TMG:</strong></p>
            <p>Emran Khan<br>E-Mail: emran@example.com</p>
            <br>
            <p><strong>Datenschutzerklärung:</strong> Der Schutz Ihrer persönlichen Daten ist uns wichtig. Diese Webseite entspricht den Vorgaben der DSGVO (Datenschutz-Grundverordnung).</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-container">
            <p>&copy; 2026 GesundheitsDE. Alle Rechte vorbehalten.</p>
            <p class="disclaimer">*Hinweis: Die dargestellten Ergebnisse sind individuell und können variieren. Bei gesundheitlichen Fragen konsultieren Sie bitte Ihren Arzt.</p>
            <div class="footer-links">
                <a href="#impressum">Impressum</a> | 
                <a href="#impressum">Datenschutz</a> | 
                <a href="#impressum">Affiliate-Offenlegung</a>
            </div>
        </div>
    </footer>

</body>
</html>