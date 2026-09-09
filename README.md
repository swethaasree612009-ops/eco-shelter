# eco-shelter
Climate-responsive eco shelter design for extreme climatic regions
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Eco Shelter | Climate Responsive Shelter Design</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #f4f8f3;
            color: #26352b;
        }

        header {
            background: #174d32;
            color: white;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-size: 14px;
        }

        .hero {
            min-height: 85vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 50px 20px;
            background: linear-gradient(135deg, #e8f4e9, #ffffff);
        }

        .hero-content {
            max-width: 800px;
        }

        .hero h1 {
            font-size: 52px;
            color: #174d32;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 19px;
            line-height: 1.7;
            color: #53645a;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            padding: 14px 25px;
            background: #23844d;
            color: white;
            text-decoration: none;
            border-radius: 8px;
            font-weight: bold;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background: #176238;
        }

        section {
            padding: 70px 8%;
        }

        .section-title {
            text-align: center;
            color: #174d32;
            font-size: 34px;
            margin-bottom: 15px;
        }

        .section-subtitle {
            text-align: center;
            color: #68766d;
            margin-bottom: 40px;
        }

        .form-container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
        }

        label {
            display: block;
            margin-top: 18px;
            margin-bottom: 7px;
            font-weight: bold;
        }

        input, select {
            width: 100%;
            padding: 13px;
            border: 1px solid #ccd8cf;
            border-radius: 7px;
            font-size: 15px;
        }

        .dimensions {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .card {
            background: white;
            padding: 25px;
            border-radius: 14px;
            box-shadow: 0 5px 18px rgba(0,0,0,0.07);
        }

        .card h3 {
            color: #23844d;
            margin-bottom: 12px;
        }

        .card p {
            color: #657269;
            line-height: 1.6;
        }

        .analysis-box {
            background: #174d32;
            color: white;
            padding: 35px;
            border-radius: 16px;
            margin-bottom: 30px;
        }

        .analysis-box h3 {
            margin-bottom: 15px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 18px;
            margin-top: 25px;
        }

        .stat {
            background: white;
            color: #26352b;
            padding: 22px;
            border-radius: 12px;
            text-align: center;
        }

        .stat strong {
            display: block;
            font-size: 28px;
            color: #23844d;
            margin-bottom: 5px;
        }

        .design {
            background: #e8f4e9;
        }

        .design-box {
            background: white;
            border-radius: 16px;
            padding: 30px;
            max-width: 900px;
            margin: auto;
        }

        .design-box ul {
            margin-top: 20px;
            padding-left: 25px;
        }

        .design-box li {
            margin-bottom: 15px;
            line-height: 1.5;
        }

        .cost-table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            border-radius: 12px;
            overflow: hidden;
        }

        .cost-table th,
        .cost-table td {
            padding: 15px;
            border-bottom: 1px solid #e1e8e2;
            text-align: left;
        }

        .cost-table th {
            background: #174d32;
            color: white;
        }

        .impact {
            background: #174d32;
            color: white;
            text-align: center;
        }

        .impact .section-title {
            color: white;
        }

        .impact p {
            max-width: 750px;
            margin: auto;
            line-height: 1.7;
        }

        footer {
            background: #102f20;
            color: white;
            text-align: center;
            padding: 25px;
        }

        @media (max-width: 700px) {
            header {
                flex-direction: column;
                gap: 12px;
            }

            nav a {
                margin: 0 7px;
            }

            .hero h1 {
                font-size: 38px;
            }

            .dimensions {
                grid-template-columns: 1fr;
            }

            section {
                padding: 50px 5%;
            }
        }
    </style>
</head>

<body>

<header>
    <div class="logo">🌱 Eco Shelter</div>

    <nav>
        <a href="#home">Home</a>
        <a href="#climate">Climate</a>
        <a href="#design">Design</a>
        <a href="#materials">Materials</a>
        <a href="#results">Results</a>
    </nav>
</header>


<!-- HOME -->
<section class="hero" id="home">

    <div class="hero-content">

        <h1>Climate-Responsive Eco Shelter</h1>

        <p>
            Design sustainable shelters according to the climate,
            location, budget and requirements of the people.
        </p>

        <a href="#input" class="btn">
            Start Shelter Analysis →
        </a>

    </div>

</section>


<!-- INPUT -->
<section id="input">

    <h2 class="section-title">Tell us about your shelter</h2>

    <p class="section-subtitle">
        A few details help us understand your requirements and create
        a suitable climate-responsive shelter.
    </p>

    <div class="form-container">

        <label>Shelter Location</label>
        <input
            type="text"
            placeholder="Enter city / district / location"
            value="Ladakh"
        >

        <label>Number of Occupants</label>
        <input
            type="number"
            value="4"
            min="1"
        >

        <label>Estimated Budget (₹)</label>
        <input
            type="number"
            placeholder="Example: 300000"
        >

        <label>Shelter Dimensions (metres)</label>

        <div class="dimensions">
            <input type="number" placeholder="Length">
            <input type="number" placeholder="Width">
            <input type="number" placeholder="Height">
        </div>

        <label>Shelter Type</label>

        <select>
            <option>Emergency / Disaster Relief</option>
            <option>Temporary / Tent Shelter</option>
            <option>Rural / Low-Cost Shelter</option>
            <option>Permanent Small Residential</option>
            <option>Community Shelter</option>
        </select>

        <br><br>

        <a href="#climate" class="btn">
            Analyze Climate & Get Design →
        </a>

    </div>

</section>


<!-- CLIMATE -->
<section id="climate">

    <h2 class="section-title">Climate Analysis</h2>

    <p class="section-subtitle">
        Understanding the local climate helps us select the right shelter design.
    </p>

    <div class="analysis-box">

        <h3>📍 Location: Ladakh</h3>

        <p>
            The selected region experiences extreme temperature variation,
            strong solar radiation, cold nights and dry winds.
        </p>

        <div class="stats">

            <div class="stat">
                <strong>-15°C</strong>
                Night Temperature
            </div>

            <div class="stat">
                <strong>15°C</strong>
                Day Temperature
            </div>

            <div class="stat">
                <strong>High</strong>
                Solar Radiation
            </div>

            <div class="stat">
                <strong>Cold</strong>
                Night Conditions
            </div>

        </div>

    </div>

    <div class="cards">

        <div class="card">
            <h3>☀️ Solar Radiation</h3>
            <p>
                Strong sunlight can provide useful heat during the daytime.
            </p>
        </div>

        <div class="card">
            <h3>🌬️ Wind</h3>
            <p>
                Cold winds increase heat loss through openings and external surfaces.
            </p>
        </div>

        <div class="card">
            <h3>🌡️ Temperature</h3>
            <p>
                Large day-night temperature differences require good insulation.
            </p>
        </div>

        <div class="card">
            <h3>🏔️ Altitude</h3>
            <p>
                High-altitude conditions influence material and shelter selection.
            </p>
        </div>

    </div>

</section>


<!-- DESIGN -->
<section class="design" id="design">

    <h2 class="section-title">Recommended Eco Shelter Design</h2>

    <p class="section-subtitle">
        A passive and climate-responsive design approach.
    </p>

    <div class="design-box">

        <h3>🏠 Suggested Design Features</h3>

        <ul>

            <li>
                <b>South-facing windows:</b>
                Capture useful sunlight during the daytime.
            </li>

            <li>
                <b>Thick insulated walls:</b>
                Reduce heat transfer between indoors and outdoors.
            </li>

            <li>
                <b>Roof insulation:</b>
                Minimizes heat loss through the roof.
            </li>

            <li>
                <b>Thermal mass:</b>
                Helps store daytime heat and release it gradually.
            </li>

            <li>
                <b>Controlled ventilation:</b>
                Provides fresh air while reducing unnecessary heat loss.
            </li>

            <li>
                <b>Small protected openings:</b>
                Reduce exposure to cold winds.
            </li>

        </ul>

    </div>

</section>


<!-- MATERIALS -->
<section id="materials">

    <h2 class="section-title">Materials & Estimated Cost</h2>

    <p class="section-subtitle">
        Sustainable and locally suitable construction materials.
    </p>

    <table class="cost-table">

        <tr>
            <th>Material</th>
            <th>Purpose</th>
            <th>Estimated Cost</th>
        </tr>

        <tr>
            <td>Local Stone</td>
            <td>Strong wall construction</td>
            <td>₹60,000</td>
        </tr>

        <tr>
            <td>Mud / Adobe</td>
            <td>Thermal mass and insulation</td>
            <td>₹40,000</td>
        </tr>

        <tr>
            <td>Insulation</td>
            <td>Reduce heat loss</td>
            <td>₹35,000</td>
        </tr>

        <tr>
            <td>Timber</td>
            <td>Doors and structural elements</td>
            <td>₹30,000</td>
        </tr>

        <tr>
            <td>Roofing</td>
            <td>Weather protection</td>
            <td>₹45,000</td>
        </tr>

        <tr>
            <th colspan="2">Approximate Total</th>
            <th>₹2,10,000</th>
        </tr>

    </table>

    <br>

    <p style="text-align:center;">
        *Cost values are prototype estimates and may vary according to location,
        material availability and construction requirements.
    </p>

</section>


<!-- RESULTS -->
<section class="impact" id="results">

    <h2 class="section-title">Results & Environmental Impact</h2>

    <p>
        The proposed Eco Shelter focuses on thermal comfort,
        reduced heat loss and sustainable construction.
        Climate-responsive planning can improve indoor comfort
        while reducing dependence on external heating energy.
    </p>

    <br><br>

    <div class="cards">

        <div class="card">
            <h3>🌡️ Better Comfort</h3>
            <p>
                Helps maintain a more comfortable indoor environment.
            </p>
        </div>

        <div class="card">
            <h3>♻️ Eco Friendly</h3>
            <p>
                Encourages the use of sustainable and locally available materials.
            </p>
        </div>

        <div class="card">
            <h3>🔥 Less Heat Loss</h3>
            <p>
                Insulation and passive design reduce unnecessary heat transfer.
            </p>
        </div>

        <div class="card">
            <h3>💰 Cost Efficient</h3>
            <p>
                Climate-based planning can help make construction more efficient.
            </p>
        </div>

    </div>

</section>


<footer>

    <p>
        © 2026 Eco Shelter | Climate-Responsive Sustainable Design
    </p>

</footer>

</body>
</html>