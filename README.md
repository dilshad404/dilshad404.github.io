<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>My Goal Calendar</title>
    <style>
        :root {
            --bg-color: #0a0a0a;
            --text-color: #ffffff;
            --accent-color: #007AFF; /* iOS Blue */
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            width: 1179px; /* Exact iPhone 15 Pro Width */
            height: 2556px; /* Exact iPhone 15 Pro Height */
            overflow: hidden;
            display: flex;
            flex-direction: column;
        }

        /* 1. CLOCK SAFE AREA (Top 25%) */
        .spacer-top {
            height: 25%; 
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            color: #333; /* Dim text for the area behind the clock */
        }

        /* 2. MAIN GOAL AREA */
        .content {
            flex: 1;
            padding: 60px;
            display: flex;
            flex-direction: column;
            gap: 40px;
        }

        .header {
            font-size: 64px;
            font-weight: 800;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 20px;
        }

        .goal-card {
            background: #1c1c1e;
            padding: 40px;
            border-radius: 30px;
            border-left: 10px solid var(--accent-color);
        }

        .goal-title {
            font-size: 48px;
            font-weight: 600;
            margin-bottom: 10px;
        }

        .goal-status {
            font-size: 32px;
            color: #8e8e93;
        }

        /* 3. BOTTOM INFO (Avoids the Home Bar) */
        .footer {
            height: 150px;
            text-align: center;
            font-size: 28px;
            color: #444;
        }

        .progress-bar {
            width: 100%;
            height: 20px;
            background: #333;
            border-radius: 10px;
            margin-top: 20px;
        }

        .progress-fill {
            width: 70%; /* Dynamic value */
            height: 100%;
            background: var(--accent-color);
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <div class="spacer-top">Content starts below the clock</div>

    <div class="content">
        <div class="header">Daily Focus</div>

        <div class="goal-card">
            <div class="goal-title">🚀 Odoo 19 Migration</div>
            <div class="goal-status">Current Task: Custom Module Testing</div>
            <div class="progress-bar"><div class="progress-fill" style="width: 45%;"></div></div>
        </div>

        <div class="goal-card">
            <div class="goal-title">🏢 Bixolve Setup</div>
            <div class="goal-status">Subdomain & Branding</div>
            <div class="progress-bar"><div class="progress-fill" style="width: 80%;"></div></div>
        </div>

        <div class="goal-card">
            <div class="goal-title">🍎 Workout App Dev</div>
            <div class="goal-status">Rep Tracking Logic</div>
            <div class="progress-bar"><div class="progress-fill" style="width: 20%;"></div></div>
        </div>
    </div>

    <div class="footer">
        Last updated: Feb 19, 2026
    </div>

</body>
</html>
