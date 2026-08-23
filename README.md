<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Syntropy - Hybrid Athlete Mobile OS</title>
</head>
<body style="background-color: #0b0f17; color: #c9d1d9; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; line-height: 1.6; padding: 20px; max-width: 1000px; margin: 0 auto;">

  <!-- HEADER / BANNER -->
  <div align="center" style="border-bottom: 1px solid #21262d; padding-bottom: 28px; margin-bottom: 32px;">
    <h1 style="color: #ffffff; font-size: 2.8rem; margin-bottom: 8px; letter-spacing: -0.5px;">
      ⚡ SYNTROPY
    </h1>
    <p style="color: #00e5ff; font-size: 1.2rem; font-weight: 600; margin-top: 0;">
      The Open-Source Mobile Platform for the Hybrid Athlete
    </p>
    <p style="color: #8b949e; max-width: 650px; margin: 12px auto;">
      A cross-platform system engineered to dynamically correlate heavy muscular volume with cardiovascular fatigue, HRV baseline shifts, and central nervous system (CNS) recovery metrics.
    </p>

    <!-- LIVE DEMO BUTTON -->
    <div style="margin: 20px 0 24px 0;">
      <a href="https://ai.studio/apps/0eb3b1b5-61ee-494f-b31b-ac2d4e7024b2?fullscreenApplet=true" target="_blank" style="display: inline-flex; align-items: center; justify-content: center; background: linear-gradient(135deg, #00e5ff 0%, #00ff66 100%); color: #0b0f17; font-weight: 700; padding: 12px 28px; border-radius: 8px; text-decoration: none; font-size: 1.05rem; box-shadow: 0 4px 20px rgba(0, 229, 255, 0.35); transition: transform 0.2s ease;">
        🚀 Try Live App Demo
      </a>
    </div>
    
    <!-- TECH BADGES -->
    <div>
      <span style="background: #1f2937; color: #38bdf8; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">Flutter 3.x</span>
      <span style="background: #1f2937; color: #4ade80; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">NestJS</span>
      <span style="background: #1f2937; color: #a78bfa; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">TimescaleDB</span>
      <span style="background: #1f2937; color: #f43f5e; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">HealthKit / Google Health Connect</span>
      <span style="background: #1f2937; color: #fbbf24; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold;">MVVM Architecture</span>
    </div>
  </div>

  <!-- TABLE OF CONTENTS -->
  <div style="background: #161b22; border: 1px solid #30363d; border-radius: 8px; padding: 20px; margin-bottom: 32px;">
    <h3 style="color: #f0f6fc; margin-top: 0;">📋 Table of Contents</h3>
    <ul style="padding-left: 20px; margin-bottom: 0;">
      <li><a href="#demo" style="color: #58a6ff; text-decoration: none;">Interactive Live Demo</a></li>
      <li><a href="#overview" style="color: #58a6ff; text-decoration: none;">Executive Overview</a></li>
      <li><a href="#architecture" style="color: #58a6ff; text-decoration: none;">System Architecture</a></li>
      <li><a href="#features" style="color: #58a6ff; text-decoration: none;">Core Features</a></li>
      <li><a href="#wearables" style="color: #58a6ff; text-decoration: none;">Wearable Integration Matrix</a></li>
      <li><a href="#tech-stack" style="color: #58a6ff; text-decoration: none;">Technical Stack & Specifications</a></li>
      <li><a href="#quickstart" style="color: #58a6ff; text-decoration: none;">Quickstart & Local Environment</a></li>
    </ul>
  </div>

  <!-- INTERACTIVE DEMO SECTION -->
  <div id="demo" style="margin-bottom: 40px; background: #161b22; border: 1px solid #00e5ff33; border-radius: 8px; padding: 20px;">
    <h2 style="color: #00e5ff; margin-top: 0;">🌐 Interactive Live Demo</h2>
    <p>
      Explore the web-based interactive model of the Syntropy application directly in your browser:
    </p>
    <p>
      👉 <a href="https://ai.studio/apps/0eb3b1b5-61ee-494f-b31b-ac2d4e7024b2?fullscreenApplet=true" target="_blank" style="color: #00ff66; font-weight: bold; text-decoration: underline;">Launch Fullscreen Web App</a>
    </p>
  </div>

  <!-- EXECUTIVE OVERVIEW -->
  <div id="overview" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🚀 Executive Overview</h2>
    <p>
      Traditional fitness applications suffer from strict domain segregation: platforms like <em>Strava</em> excel exclusively at endurance logging, while apps like <em>Strong</em> focus solely on strength metrics. Neither accounts for the physiological stress that high-volume resistance training imposes on cardiovascular output, nor how depleted <strong>Heart Rate Variability (HRV)</strong> reduces mechanical power output.
    </p>
    <p>
      <strong>Syntropy</strong> solves this gap by offering a single telemetry pipeline that ingests continuous biometric data from native smartwatch frameworks and third-party APIs, computing a real-time <strong>Readiness Score (0–100)</strong> to dynamically adapt workout loads.
    </p>
  </div>

  <!-- SYSTEM ARCHITECTURE -->
  <div id="architecture" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🏗️ System Architecture</h2>
    <p>The system follows an event-driven microservices topology built to ingest and process high-frequency time-series biometric data.</p>
    
    <div style="background: #0d1117; border: 1px solid #30363d; border-radius: 6px; padding: 16px; font-family: monospace; overflow-x: auto; font-size: 0.9rem; color: #7ee787;">
<pre style="margin: 0;">
[ Apple HealthKit / Wear OS ]    [ Garmin / Whoop Webhooks ]
             │                                │
             ▼                                ▼
  (Native Client SDK)             (AWS API Gateway)
             │                                │
      [ Local SQLite ]                [ AWS SQS Queue ]
   (WatermelonDB Sync Engine)                 │
             │                                ▼
             └──────────────► [ NestJS GraphQL API Node ]
                                      │
                                      ▼
                          [ PostgreSQL + TimescaleDB ]
</pre>
    </div>
  </div>

  <!-- CORE FEATURES -->
  <div id="features" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">⚡ Core Features</h2>
    
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin-top: 20px;">
      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #00e5ff; margin-top: 0;">📊 Dynamic Readiness Score</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Calculates daily readiness using a rolling 14-day Z-Score baseline across rMSSD HRV, Resting Heart Rate, and Deep/REM sleep ratios.
        </p>
      </div>

      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #00ff66; margin-top: 0;">🏋️‍♂️ Dual-Engine HUD</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Low-latency HUD interface featuring dynamic HR Zone color illumination and tap-and-hold set logging optimized for sweaty environments.
        </p>
      </div>

      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #ff0055; margin-top: 0;">📈 Hybrid Data Overlay</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Dual-axis charts plotting total weight room tonnage directly against HRV suppression curves to isolate overtraining triggers.
        </p>
      </div>
    </div>
  </div>

  <!-- WEARABLE INTEGRATION MATRIX -->
  <div id="wearables" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">⌚ Wearable Integration Matrix</h2>
    
    <table style="width: 100%; border-collapse: collapse; margin-top: 16px; text-align: left; font-size: 0.9rem;">
      <thead>
        <tr style="background-color: #161b22; border-bottom: 2px solid #30363d;">
          <th style="padding: 10px; color: #f0f6fc;">Provider</th>
          <th style="padding: 10px; color: #f0f6fc;">Integration Method</th>
          <th style="padding: 10px; color: #f0f6fc;">Data Ingest Points</th>
          <th style="padding: 10px; color: #f0f6fc;">Sync Priority</th>
        </tr>
      </thead>
      <tbody>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #38bdf8;">Apple HealthKit</td>
          <td style="padding: 10px;">Native Swift / HKObserverQuery</td>
          <td style="padding: 10px;">HRV (SDNN), Active HR, Sleep Stages, Active Energy</td>
          <td style="padding: 10px; color: #4ade80;">Primary (Native)</td>
        </tr>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #a3e635;">Google Health Connect</td>
          <td style="padding: 10px;">Native Kotlin / Health Connect SDK</td>
          <td style="padding: 10px;">Heart Rate, Sleep Duration, Steps, VO2 Max</td>
          <td style="padding: 10px; color: #4ade80;">Primary (Native)</td>
        </tr>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #fbbf24;">Garmin Connect</td>
          <td style="padding: 10px;">OAuth2 / Server Push Webhooks</td>
          <td style="padding: 10px;">Respiration, Body Battery, Advanced GPS Metrics</td>
          <td style="padding: 10px; color: #fbbf24;">Secondary (Server)</td>
        </tr>
        <tr>
          <td style="padding: 10px; font-weight: bold; color: #f43f5e;">WHOOP & Oura</td>
          <td style="padding: 10px;">REST API / Nightly Sync Batch</td>
          <td style="padding: 10px;">Recovery Score, Sleep Staging, Skin Temp, rMSSD</td>
          <td style="padding: 10px; color: #f43f5e;">Tertiary (API)</td>
        </tr>
      </tbody>
    </table>
  </div>

  <!-- TECHNICAL STACK SPECIFICATIONS -->
  <div id="tech-stack" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🛠️ Technical Specifications</h2>
    
    <ul style="line-height: 1.8;">
      <li><strong>Client Layer:</strong> Flutter 3.x using the Impeller rendering engine, structured around strict <code>MVVM</code> design patterns and <code>Riverpod</code> for decoupled state management.</li>
      <li><strong>Local Database:</strong> SQLite managed via <code>WatermelonDB</code> primitives, delivering offline-first persistence with delta-based vector clock synchronization.</li>
      <li><strong>Backend Layer:</strong> NestJS application instance exposing a unified <code>GraphQL</code> interface alongside REST endpoints for high-throughput webhook processing.</li>
      <li><strong>Database Layer:</strong> PostgreSQL augmented with the <code>TimescaleDB</code> extension, designed specifically for dynamic time-series aggregation of heart-rate arrays.</li>
    </ul>
  </div>

  <!-- QUICKSTART -->
  <div id="quickstart" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🚀 Quickstart & Local Environment</h2>
    
    <p>To set up the development client locally, clone the repository and execute the bootstrapping commands:</p>

    <div style="background: #0d1117; border: 1px solid #30363d; border-radius: 6px; padding: 16px; font-family: monospace; color: #e6edf3; font-size: 0.85rem; overflow-x: auto;">
      <p style="margin: 0; color: #8b949e;"># Clone the repository</p>
      <p style="margin: 0;">git clone https://github.com/your-org/syntropy-mobile-app.git</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Navigate to client directory and fetch dependencies</p>
      <p style="margin: 0;">cd syntropy-mobile-app/client && flutter pub get</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Run unit test suite</p>
      <p style="margin: 0;">flutter test</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Target iOS simulator (requires Xcode configured for HealthKit)</p>
      <p style="margin: 0;">flutter run -d iphone</p>
    </div>
  </div>

  <!-- FOOTER -->
  <div align="center" style="border-top: 1px solid #21262d; padding-top: 24px; color: #8b949e; font-size: 0.85rem;">
    <p>Syntropy Engine · Released under the Apache 2.0 License · <a href="https://ai.studio/apps/0eb3b1b5-61ee-494f-b31b-ac2d4e7024b2?fullscreenApplet=true" target="_blank" style="color: #00e5ff; text-decoration: none;">Try App Demo</a></p>
  </div>

</body>
</html>
      A cross-platform system engineered to dynamically correlate heavy muscular volume with cardiovascular fatigue, HRV baseline shifts, and central nervous system (CNS) recovery metrics.
    </p>
    
    <!-- TECH BADGES -->
    <div style="margin-top: 20px;">
      <span style="background: #1f2937; color: #38bdf8; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">Flutter 3.x</span>
      <span style="background: #1f2937; color: #4ade80; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">NestJS</span>
      <span style="background: #1f2937; color: #a78bfa; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">TimescaleDB</span>
      <span style="background: #1f2937; color: #f43f5e; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold; margin-right: 6px;">HealthKit / Google Health Connect</span>
      <span style="background: #1f2937; color: #fbbf24; padding: 4px 10px; border-radius: 12px; font-size: 0.85rem; font-weight: bold;">MVVM Architecture</span>
    </div>
  </div>

  <!-- TABLE OF CONTENTS -->
  <div style="background: #161b22; border: 1px solid #30363d; border-radius: 8px; padding: 20px; margin-bottom: 32px;">
    <h3 style="color: #f0f6fc; margin-top: 0;">📋 Table of Contents</h3>
    <ul style="padding-left: 20px; margin-bottom: 0;">
      <li><a href="#overview" style="color: #58a6ff; text-decoration: none;">Executive Overview</a></li>
      <li><a href="#architecture" style="color: #58a6ff; text-decoration: none;">System Architecture</a></li>
      <li><a href="#features" style="color: #58a6ff; text-decoration: none;">Core Features</a></li>
      <li><a href="#wearables" style="color: #58a6ff; text-decoration: none;">Wearable Integration Matrix</a></li>
      <li><a href="#tech-stack" style="color: #58a6ff; text-decoration: none;">Technical Stack & Specifications</a></li>
      <li><a href="#quickstart" style="color: #58a6ff; text-decoration: none;">Quickstart & Local Environment</a></li>
    </ul>
  </div>

  <!-- EXECUTIVE OVERVIEW -->
  <div id="overview" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🚀 Executive Overview</h2>
    <p>
      Traditional fitness applications suffer from strict domain segregation: platforms like <em>Strava</em> excel exclusively at endurance logging, while apps like <em>Strong</em> focus solely on strength metrics. Neither accounts for the physiological stress that high-volume resistance training imposes on cardiovascular output, nor how depleted <strong>Heart Rate Variability (HRV)</strong> reduces mechanical power output.
    </p>
    <p>
      <strong>Syntropy</strong> solves this gap by offering a single telemetry pipeline that ingests continuous biometric data from native smartwatch frameworks and third-party APIs, computing a real-time <strong>Readiness Score (0–100)</strong> to dynamically adapt workout loads.
    </p>
  </div>

  <!-- SYSTEM ARCHITECTURE -->
  <div id="architecture" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🏗️ System Architecture</h2>
    <p>The system follows an event-driven microservices topology built to ingest and process high-frequency time-series biometric data.</p>
    
    <div style="background: #0d1117; border: 1px solid #30363d; border-radius: 6px; padding: 16px; font-family: monospace; overflow-x: auto; font-size: 0.9rem; color: #7ee787;">
<pre style="margin: 0;">
[ Apple HealthKit / Wear OS ]    [ Garmin / Whoop Webhooks ]
             │                                │
             ▼                                ▼
  (Native Client SDK)             (AWS API Gateway)
             │                                │
      [ Local SQLite ]                [ AWS SQS Queue ]
   (WatermelonDB Sync Engine)                 │
             │                                ▼
             └──────────────► [ NestJS GraphQL API Node ]
                                      │
                                      ▼
                          [ PostgreSQL + TimescaleDB ]
</pre>
    </div>
  </div>

  <!-- CORE FEATURES -->
  <div id="features" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">⚡ Core Features</h2>
    
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin-top: 20px;">
      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #00e5ff; margin-top: 0;">📊 Dynamic Readiness Score</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Calculates daily readiness using a rolling 14-day Z-Score baseline across rMSSD HRV, Resting Heart Rate, and Deep/REM sleep ratios.
        </p>
      </div>

      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #00ff66; margin-top: 0;">🏋️‍♂️ Dual-Engine HUD</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Low-latency HUD interface featuring dynamic HR Zone color illumination and tap-and-hold set logging optimized for sweaty environments.
        </p>
      </div>

      <div style="background: #161b22; border: 1px solid #30363d; border-radius: 6px; padding: 16px;">
        <h4 style="color: #ff0055; margin-top: 0;">📈 Hybrid Data Overlay</h4>
        <p style="font-size: 0.9rem; color: #8b949e; margin-bottom: 0;">
          Dual-axis charts plotting total weight room tonnage directly against HRV suppression curves to isolate overtraining triggers.
        </p>
      </div>
    </div>
  </div>

  <!-- WEARABLE INTEGRATION MATRIX -->
  <div id="wearables" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">⌚ Wearable Integration Matrix</h2>
    
    <table style="width: 100%; border-collapse: collapse; margin-top: 16px; text-align: left; font-size: 0.9rem;">
      <thead>
        <tr style="background-color: #161b22; border-bottom: 2px solid #30363d;">
          <th style="padding: 10px; color: #f0f6fc;">Provider</th>
          <th style="padding: 10px; color: #f0f6fc;">Integration Method</th>
          <th style="padding: 10px; color: #f0f6fc;">Data Ingest Points</th>
          <th style="padding: 10px; color: #f0f6fc;">Sync Priority</th>
        </tr>
      </thead>
      <tbody>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #38bdf8;">Apple HealthKit</td>
          <td style="padding: 10px;">Native Swift / HKObserverQuery</td>
          <td style="padding: 10px;">HRV (SDNN), Active HR, Sleep Stages, Active Energy</td>
          <td style="padding: 10px; color: #4ade80;">Primary (Native)</td>
        </tr>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #a3e635;">Google Health Connect</td>
          <td style="padding: 10px;">Native Kotlin / Health Connect SDK</td>
          <td style="padding: 10px;">Heart Rate, Sleep Duration, Steps, VO2 Max</td>
          <td style="padding: 10px; color: #4ade80;">Primary (Native)</td>
        </tr>
        <tr style="border-bottom: 1px solid #21262d;">
          <td style="padding: 10px; font-weight: bold; color: #fbbf24;">Garmin Connect</td>
          <td style="padding: 10px;">OAuth2 / Server Push Webhooks</td>
          <td style="padding: 10px;">Respiration, Body Battery, Advanced GPS Metrics</td>
          <td style="padding: 10px; color: #fbbf24;">Secondary (Server)</td>
        </tr>
        <tr>
          <td style="padding: 10px; font-weight: bold; color: #f43f5e;">WHOOP & Oura</td>
          <td style="padding: 10px;">REST API / Nightly Sync Batch</td>
          <td style="padding: 10px;">Recovery Score, Sleep Staging, Skin Temp, rMSSD</td>
          <td style="padding: 10px; color: #f43f5e;">Tertiary (API)</td>
        </tr>
      </tbody>
    </table>
  </div>

  <!-- TECHNICAL STACK SPECIFICATIONS -->
  <div id="tech-stack" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🛠️ Technical Specifications</h2>
    
    <ul style="line-height: 1.8;">
      <li><strong>Client Layer:</strong> Flutter 3.x using the Impeller rendering engine, structured around strict <code>MVVM</code> design patterns and <code>Riverpod</code> for decoupled state management.</li>
      <li><strong>Local Database:</strong> SQLite managed via <code>WatermelonDB</code> primitives, delivering offline-first persistence with delta-based vector clock synchronization.</li>
      <li><strong>Backend Layer:</strong> NestJS application instance exposing a unified <code>GraphQL</code> interface alongside REST endpoints for high-throughput webhook processing.</li>
      <li><strong>Database Layer:</strong> PostgreSQL augmented with the <code>TimescaleDB</code> extension, designed specifically for dynamic time-series aggregation of heart-rate arrays.</li>
    </ul>
  </div>

  <!-- QUICKSTART -->
  <div id="quickstart" style="margin-bottom: 40px;">
    <h2 style="color: #f0f6fc; border-bottom: 1px solid #21262d; padding-bottom: 8px;">🚀 Quickstart & Local Environment</h2>
    
    <p>To set up the development client locally, clone the repository and execute the bootstrapping commands:</p>

    <div style="background: #0d1117; border: 1px solid #30363d; border-radius: 6px; padding: 16px; font-family: monospace; color: #e6edf3; font-size: 0.85rem; overflow-x: auto;">
      <p style="margin: 0; color: #8b949e;"># Clone the repository</p>
      <p style="margin: 0;">git clone https://github.com/your-org/syntropy-mobile-app.git</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Navigate to client directory and fetch dependencies</p>
      <p style="margin: 0;">cd syntropy-mobile-app/client && flutter pub get</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Run unit test suite</p>
      <p style="margin: 0;">flutter test</p>
      <br />
      <p style="margin: 0; color: #8b949e;"># Target iOS simulator (requires Xcode configured for HealthKit)</p>
      <p style="margin: 0;">flutter run -d iphone</p>
    </div>
  </div>

  <!-- FOOTER -->
  <div align="center" style="border-top: 1px solid #21262d; padding-top: 24px; color: #8b949e; font-size: 0.85rem;">
    <p>Syntropy Engine · Released under the Apache 2.0 License</p>
  </div>

</body>
</html>
