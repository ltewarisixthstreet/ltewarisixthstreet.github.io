# "Demo page for Jonathan"

<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Artisan Walls - Premium Finishes Prototype</title>
    <body> Schedule your personalized consultation today.  Embark on a journey to create your whole-home renovation in the Austin area. Our master builders are ready to bring your unique vision to life, blending timeless elegance with modern luxury. </body>
    <style>
        :root {
            --bg-color: #fcfbfa;
            --text-dark: #2e2d2c;
            --text-light: #706e6b;
            --accent: #8c8275;
            --card-bg: #f4f1ec;
            --border: #e3ded7;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-dark);
            line-height: 1.6;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 3rem;
            border-bottom: 1px solid var(--border);
            padding-bottom: 2rem;
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 300;
            letter-spacing: -0.03em;
            color: var(--text-dark);
            margin-bottom: 0.5rem;
        }

        header p {
            color: var(--text-light);
            font-size: 1.1rem;
        }

        .badge {
            display: inline-block;
            background: var(--accent);
            color: white;
            padding: 0.25rem 0.75rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }

        .grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
            margin-bottom: 3rem;
        }

        @media (min-width: 768px) {
            .grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .card {
            background: var(--card-bg);
            border: 1px solid var(--border);
            border-radius: 8px;
            padding: 2rem;
            transition: transform 0.2s ease;
        }

        .card:hover {
            transform: translateY(-2px);
        }

        .card h2 {
            font-size: 1.4rem;
            font-weight: 500;
            margin-bottom: 1rem;
            color: var(--text-dark);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .price-tag {
            font-size: 0.9rem;
            background: #e6e1da;
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            color: var(--accent);
            font-weight: 600;
        }

        .card p {
            color: var(--text-light);
            margin-bottom: 1.5rem;
            font-size: 0.95rem;
        }

        /* Interactive Texture Simulator */
        .texture-preview {
            height: 120px;
            border-radius: 6px;
            margin-bottom: 1rem;
            border: 1px solid var(--border);
            position: relative;
            overflow: hidden;
        }

        .limewash-smooth {
            background: rgb(238,235,230);
            background: radial-gradient(circle, rgba(238,235,230,1) 0%, rgba(222,217,209,1) 70%, rgba(207,200,191,1) 100%);
            box-shadow: inset 0 0 20px rgba(0,0,0,0.05);
        }

        .limewash-textured {
            background: #ded9d1;
            background-image: 
                radial-gradient(rgba(255,255,255,0.4) 1px, transparent 0),
                radial-gradient(rgba(0,0,0,0.05) 1px, transparent 0);
            background-size: 8px 8px;
            background-position: 0 0, 4px 4px;
        }

        /* Interactive Cost Calculator */
        .calculator {
            background: #fff;
            border: 2px solid var(--border);
            border-radius: 8px;
            padding: 2.5rem;
            margin-top: 3rem;
        }

        .calculator h3 {
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            font-weight: 500;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            font-size: 0.9rem;
        }

        select, input {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid var(--border);
            border-radius: 4px;
            background: var(--bg-color);
            font-size: 1rem;
            color: var(--text-dark);
        }

        .calc-result {
            background: var(--card-bg);
            padding: 1.5rem;
            border-radius: 6px;
            margin-top: 1.5rem;
            text-align: center;
        }

        .calc-result span {
            display: block;
            font-size: 2rem;
            font-weight: 600;
            color: var(--accent);
            margin-top: 0.5rem;
        }

        footer {
            text-align: center;
            margin-top: 4rem;
            font-size: 0.85rem;
            color: var(--text-light);
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <span class="badge">Concept Prototype</span>
        <h1>Artisan Wall Systems</h1>
        <p>A specialized companion brand for General Contractors offering premium wall finishes.</p>
    </header>

    <main>
        <div class="grid">
            <!-- Service 1 -->
            <div class="card">
                <h2>Limewash Over Level 5 <span class="price-tag">Premium</span></h2>
                <p>A flawless skim-coat application bringing zero-texture drywall to a seamless, velvet-like finish. Perfect for soft, glowing mineral paints.</p>
                <div class="texture-preview limewash-smooth"></div>
                <p style="font-size: 0.85rem; font-style: italic;">Visual Profile: Smooth matte finish with subtle, organic color mottling.</p>
            </div>

            <!-- Service 2 -->
            <div class="card">
                <h2>Skip Trowel + Mineral Wash <span class="price-tag">Artisan</span></h2>
                <p>Hand-applied drywall compound that mimics historic European plaster work. The multi-layered limewash catches the depth of the trowel skips.</p>
                <div class="texture-preview limewash-textured"></div>
                <p style="font-size: 0.85rem; font-style: italic;">Visual Profile: Highly tactile, dramatic shadows, old-world aesthetic.</p>
            </div>
        </div>

        <!-- Interactive Pricing Calculator Component -->
        <div class="calculator">
            <h3>Interactive Estimate Simulator</h3>
            <p style="color: var(--text-light); margin-bottom: 1.5rem; font-size: 0.9rem;">
                Show your prospective clients or designer partners a baseline price instantly during walk-throughs.
            </p>
            
            <div class="form-group">
                <label for="finishType">Select Finish System</label>
                <select id="finishType" onchange="calculateEstimate()">
                    <option value="9">Limewash over Acrylic Quartz Primer ($9 / sq ft)</option>
                    <option value="14">Level 5 Drywall Smooth Prep + Limewash ($14 / sq ft)</option>
                    <option value="18">Hand-Troweled Roman Clay / Micro-Plaster ($18 / sq ft)</option>
                </select>
            </div>

            <div class="form-group">
                <label for="wallSize">Estimated Wall Area (Square Footage)</label>
                <input type="number" id="wallSize" value="150" min="10" oninput="calculateEstimate()">
            </div>

            <div class="calc-result">
                <strong>Estimated Bid Range (Labor & Materials)</strong>
                <span id="totalEstimate">$1,350 - $1,620</span>
            </div>
        </div>
    </main>

    <footer>
        <p>Artisan Walls Concept &bull; Built to demonstrate high-margin scaling options for General Contractors.</p>
    </footer>
</div>

<script>
    function calculateEstimate() {
        const ratePerSqFt = parseFloat(document.getElementById('finishType').value);
        const sqFt = parseFloat(document.getElementById('wallSize').value) || 0;
        
        const basePrice = ratePerSqFt * sqFt;
        // Provide an artisan high-low range to preserve margins
        const lowRange = Math.round(basePrice);
        const highRange = Math.round(basePrice * 1.2);

        if(sqFt === 0) {
            document.getElementById('totalEstimate').innerText = "$0";
            return;
        }

        document.getElementById('totalEstimate').innerText = 
            `$${lowRange.toLocaleString()} - $${highRange.toLocaleString()}`;
    }
</script>

</body>
</html>
