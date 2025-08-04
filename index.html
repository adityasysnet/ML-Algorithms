<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ML Algorithm Tracker</title>
  <link href="https://cdn.jsdelivr.net/npm/remixicon@4.0.0/fonts/remixicon.css" rel="stylesheet">
  <style>
    :root {
      --bg: #0d1117;
      --section-bg: #161b22;
      --text: #c9d1d9;
      --highlight: #3fb950;
    }
    .theme-light {
      --bg: #f3f4f6;
      --section-bg: #ffffff;
      --text: #1f2937;
      --highlight: #10b981;
    }
    .theme-blue {
      --bg: #0a0e2a;
      --section-bg: #12163c;
      --text: #e0e7ff;
      --highlight: #60a5fa;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: var(--bg);
      color: var(--text);
      padding: 2rem;
      transition: background 0.3s, color 0.3s;
    }
    h1, h2 {
      color: var(--highlight);
      margin-bottom: 1rem;
    }
    .section {
      margin-bottom: 2rem;
      padding: 1rem;
      background-color: var(--section-bg);
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(63, 185, 80, 0.1);
    }
    .algo {
      display: flex;
      align-items: center;
      margin: 0.5rem 0;
      position: relative;
      transition: transform 0.3s ease;
    }
    .algo input {
      margin-right: 1rem;
      transform: scale(1.3);
      accent-color: var(--highlight);
    }
    .algo label {
      font-size: 1rem;
    }
    .algo.checked {
      color: var(--highlight);
      transform: scale(1.02);
    }
    .tooltip {
      position: absolute;
      background: #000000cc;
      color: white;
      padding: 4px 8px;
      font-size: 0.8rem;
      border-radius: 4px;
      top: -30px;
      left: 30px;
      white-space: nowrap;
      display: none;
    }
    .algo:hover .tooltip {
      display: block;
    }
    #themeToggle {
      position: fixed;
      top: 1rem;
      right: 1rem;
      background: var(--highlight);
      color: white;
      border: none;
      border-radius: 20px;
      padding: 0.5rem 1rem;
      cursor: pointer;
      z-index: 100;
    }
    #progressBarContainer {
      width: 100%;
      height: 6px;
      background: #333;
      border-radius: 3px;
      overflow: hidden;
      margin-bottom: 2rem;
    }
    #progressBar {
      height: 100%;
      width: 0%;
      background: var(--highlight);
      transition: width 0.3s ease-in-out;
    }
  </style>
</head>
<body class="theme-dark">
  <button id="themeToggle">Toggle Theme</button>
  <h1><i class="ri-checkbox-circle-line"></i> ML Algorithm Tracker</h1>
  <div id="progressBarContainer"><div id="progressBar"></div></div>

  <div id="tracker"></div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
  <script>
    const algoData = {
      "Supervised Learning - Classification": {
        "nb": "Naive Bayes",
        "lr": "Logistic Regression",
        "knn": "K-Nearest Neighbor",
        "rf": "Random Forest",
        "svm": "Support Vector Machine",
        "dt": "Decision Tree"
      },
      "Supervised Learning - Regression": {
        "slr": "Simple Linear Regression",
        "mlr": "Multivariate Regression",
        "lasso": "Lasso Regression"
      },
      "Unsupervised Learning - Clustering": {
        "kmeans": "K-Means Clustering",
        "dbscan": "DBSCAN",
        "pca": "Principal Component Analysis",
        "ica": "Independent Component Analysis"
      },
      "Unsupervised Learning - Association": {
        "fpg": "Frequent Pattern Growth",
        "apriori": "Apriori Algorithm"
      },
      "Unsupervised Learning - Anomaly Detection": {
        "zscore": "Z-Score Algorithm",
        "isoforest": "Isolation Forest"
      },
      "Semi-Supervised Learning": {
        "selftrain": "Self-Training",
        "cotrain": "Co-Training"
      },
      "Reinforcement Learning": {
        "policyopt": "Policy Optimization",
        "qlearn": "Q-Learning",
        "learnmodel": "Learn the Model",
        "givenmodel": "Given the Model"
      }
    };

    const tracker = document.getElementById("tracker");

    for (const section in algoData) {
      const wrapper = document.createElement("div");
      wrapper.className = "section";
      const title = document.createElement("h2");
      title.textContent = section;
      wrapper.appendChild(title);

      for (const id in algoData[section]) {
        const algoRow = document.createElement("div");
        algoRow.className = "algo";

        const cb = document.createElement("input");
        cb.type = "checkbox";
        cb.id = id;

        const label = document.createElement("label");
        label.setAttribute("for", id);
        label.textContent = algoData[section][id];

        const tooltip = document.createElement("div");
        tooltip.className = "tooltip";
        tooltip.textContent = `Learn ${algoData[section][id]}`;

        algoRow.appendChild(cb);
        algoRow.appendChild(label);
        algoRow.appendChild(tooltip);
        wrapper.appendChild(algoRow);
      }
      tracker.appendChild(wrapper);
    }

    const checkboxes = document.querySelectorAll("input[type='checkbox']");

    checkboxes.forEach(cb => {
      const key = `ml_algo_${cb.id}`;
      const row = cb.closest('.algo');
      if (localStorage.getItem(key) === "true") {
        cb.checked = true;
        row.classList.add('checked');
      }

      cb.addEventListener('change', () => {
        localStorage.setItem(key, cb.checked);
        row.classList.toggle('checked');
        updateProgress();

        if (cb.checked) {
          const pulse = document.createElement("span");
          pulse.style.position = "absolute";
          pulse.style.borderRadius = "50%";
          pulse.style.width = "20px";
          pulse.style.height = "20px";
          pulse.style.left = cb.offsetLeft + "px";
          pulse.style.top = cb.offsetTop + "px";
          pulse.style.transform = "translate(-25%, -25%)";
          pulse.style.background = "var(--highlight)";
          pulse.style.opacity = 0.3;
          pulse.style.zIndex = 2;
          document.body.appendChild(pulse);

          gsap.fromTo(pulse, { scale: 0, opacity: 0.4 }, {
            scale: 6,
            opacity: 0,
            duration: 0.6,
            ease: "power2.out",
            onComplete: () => pulse.remove()
          });
        }
      });
    });

    function updateProgress() {
      const checked = [...checkboxes].filter(cb => cb.checked).length;
      const total = checkboxes.length;
      const percent = (checked / total) * 100;
      document.getElementById("progressBar").style.width = percent + "%";
    }

    updateProgress();

    gsap.utils.toArray(".section").forEach((el, i) => {
      gsap.from(el, {
        opacity: 0,
        y: 50,
        delay: i * 0.1,
        duration: 0.6,
        ease: "power2.out",
        scrollTrigger: {
          trigger: el,
          start: "top 90%"
        }
      });
    });

    const themes = ["theme-dark", "theme-light", "theme-blue"];
    let currentTheme = 0;

    document.getElementById("themeToggle").addEventListener("click", () => {
      document.body.classList.remove(themes[currentTheme]);
      currentTheme = (currentTheme + 1) % themes.length;
      document.body.classList.add(themes[currentTheme]);
    });
  </script>
</body>
</html>
