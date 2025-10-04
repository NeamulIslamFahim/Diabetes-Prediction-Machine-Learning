<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Diabetes Prediction — Project Landing</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--accent:#06b6d4;--glass: rgba(255,255,255,0.03)}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter,ui-sans-serif,system-ui,-apple-system,'Segoe UI',Roboto,'Helvetica Neue',Arial;background:linear-gradient(180deg,#071021 0%, #0c1b2b 100%);color:#e6eef6;min-height:100vh;display:flex;align-items:center;justify-content:center;padding:24px}
    .container{width:100%;max-width:900px;background:radial-gradient(circle at 10% 10%, rgba(6,182,212,0.04), transparent 20%),var(--card);border-radius:16px;padding:36px;box-shadow:0 10px 30px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}
    header{display:flex;align-items:center;gap:16px}
    .logo{width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700;color:#042033}
    h1{margin:0;font-size:1.5rem}
    p.lead{margin:8px 0 20px;color:#bcd7e5}
    .grid{display:grid;grid-template-columns:1fr 320px;gap:20px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:12px;border:1px solid rgba(255,255,255,0.03)}
    .btn{display:inline-block;padding:12px 18px;border-radius:10px;font-weight:600;text-decoration:none;border:0;cursor:pointer}
    .btn-primary{background:var(--accent);color:#042033}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:inherit}
    .center{display:flex;gap:12px;align-items:center}
    footer{margin-top:18px;color:#98b8c8;font-size:0.9rem}
    pre{white-space:pre-wrap;background:var(--glass);padding:12px;border-radius:8px;overflow:auto;border:1px dashed rgba(255,255,255,0.02)}
    @media (max-width:880px){.grid{grid-template-columns:1fr;}.container{padding:20px}}
  </style>
</head>
<body>
  <div class="container" role="main">
    <header>
      <div class="logo">DP</div>
      <div>
        <h1>Diabetes Prediction — Project Landing</h1>
        <p class="lead">A simple landing page and README for your Diabetes Prediction notebook. Click the button to open the notebook on GitHub.</p>
      </div>
    </header>

    <div class="grid" style="margin-top:18px">
      <div class="card">
        <h3>About</h3>
        <p>This project trains machine learning models to predict diabetes from medical features (Glucose, BMI, Age, etc.). The full Jupyter notebook is hosted on GitHub — the button on the right opens it directly.</p>

        <h4 style="margin-top:12px">How to use</h4>
        <ol>
          <li>Click the "Open Notebook" button to view the notebook in GitHub.</li>
          <li>To run the notebook, you can download it (.ipynb) and open it locally or in Google Colab.</li>
          <li>If you want this landing page deployed, save this file as <code>index.html</code> and host it on GitHub Pages or Netlify.</li>
        </ol>

        <h4 style="margin-top:12px">README (preview)</h4>
        <pre># Diabetes Prediction

This repository contains a machine learning notebook that predicts whether a person
has diabetes based on medical measurements. Features include Pregnancies, Glucose,
Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, and Age.

Run the notebook to reproduce the results and view model comparison charts.

Notebook: diabetes-prediction.ipynb
</pre>

        <footer>Want a README.md file or a deployed URL? Ask and I'll provide the files ready-to-host.</footer>
      </div>

      <aside class="card" style="display:flex;flex-direction:column;align-items:stretch;justify-content:space-between">
        <div>
          <h3 style="margin-top:0">Open Notebook</h3>
          <p style="color:#bcd7e5">Click the button below to open the Jupyter notebook on GitHub (opens in a new tab).</p>
        </div>

        <div class="center" style="margin-top:12px;flex-direction:column">
          <!-- The redirect button -->
          <a class="btn btn-primary" id="open-notebook" href="https://github.com/NeamulIslamFahim/Diabetes-Prediction-Machine-Learning/blob/main/diabetes-prediction.ipynb" target="_blank" rel="noopener noreferrer" aria-label="Open Diabetes notebook on GitHub">Open Notebook on GitHub</a>

          <!-- Small secondary actions -->
          <div style="margin-top:12px;width:100%;display:flex;gap:10px">
            <a class="btn btn-ghost" href="https://github.com/NeamulIslamFahim/Diabetes-Prediction-Machine-Learning" target="_blank" rel="noopener noreferrer">View Repository</a>
            <button class="btn" id="download-readme">Download README.md</button>
          </div>
        </div>

        <small style="margin-top:12px;color:#9fb8c9">Button links point to your GitHub repository.</small>
      </aside>
    </div>
  </div>

  <script>
    // README content for download
    const readmeContent = `# Diabetes Prediction\n\nThis repository contains a Jupyter notebook (diabetes-prediction.ipynb) that trains and
compares several machine learning models to predict diabetes from medical features.\n\nFeatures:\n- Pregnancies\n- Glucose\n- BloodPressure\n- SkinThickness\n- Insulin\n- BMI\n- DiabetesPedigreeFunction\n- Age\n\nOpen the notebook here:\nhttps://github.com/NeamulIslamFahim/Diabetes-Prediction-Machine-Learning/blob/main/diabetes-prediction.ipynb\n`;

    document.getElementById('download-readme').addEventListener('click', function(){
      const blob = new Blob([readmeContent], { type: 'text/markdown' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'README.md';
      document.body.appendChild(a);
      a.click();
      a.remove();
      URL.revokeObjectURL(url);
    });
  </script>
</body>
</html>
