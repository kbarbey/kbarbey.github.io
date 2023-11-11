---
layout: page
title: Swiss Bicycle Ascents Project
permalink: /swiss-bicycle-ascents/
---

I started this project in May 2020 during Covid. The goal is to explore Switzerland's most and often least
known bicycle ascents. I extensively used the website [cols-cyclisme.com](https://www.cols-cyclisme.com/) to find the ascents and I cannot thank
them enough for their work.

# All ascents by region

<iframe src="/bikeclimbsbyregion.html" width="100%" height="300" style="border:none;"></iframe>

# Heatmap of ascents

![Subdirectory Image](/images/output.gif)

## Statistics

### Number of ascents by region

1. Alpes Valaisannes: 23/32

2. Alpes Bernoises: 17/54

3. Jura: 22/38

4. Mont-Blanc: 5/5

5. Chablais: 5/12

6. Massif de l'Ortles: 2/2

7. Alpes Uranaises: 0/17

8. Alpes Glaronaises: 0/5

9. Alpes Lépontines: 2/24

10. Alpes Rhétiques: 3/14

11. Rätikon: 0/3

12. Chaîne de la Bernina: 1/4

13. Saint-Gothard: 5/7

14. Autres: 0/2

Total: 85/244

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Optional styling for the progress bar container */
    .progress-container {
      width: 100%;
      height: 25px;
      position: relative;
    }

    progress {
      width: 100%;
      height: 100%;
      transition: all 0.2s ease-out;
        -webkit-appearance: none;
      background-image:
	    -webkit-linear-gradient(-45deg,transparent 33%, rgba(0, 0, 0, .1) 33%,rgba(0,0, 0, .1) 66%, transparent 66%),
	    -webkit-linear-gradient(top,rgba(255, 255, 255, .25),rgba(0, 0, 0, .25)),
	    -webkit-linear-gradient(left, #09c, #f44);

    border-radius: 2px; 
    background-size: 35px 20px, 100% 100%, 100% 100%;
    }

    .percentage {
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      line-height: 30px;
    }
  </style>
</head>
<body>

<!-- Example Progress Bar -->
<div class="progress-container">
  <progress id="myProgressBar" value="85" max="244"></progress>
  <div id="percentageText" class="percentage"></div>
</div>

<script>
  // Get the progress bar and percentage text elements
  var progressBar = document.getElementById('myProgressBar');
  var percentageText = document.getElementById('percentageText');

  // Update the percentage text based on the current value and max attributes
  function updatePercentage() {
    var percentage = Math.round((progressBar.value / progressBar.max) * 100);
    percentageText.textContent = percentage + '%';
  }

  // Call the updatePercentage function when the value of the progress bar changes
  progressBar.addEventListener('input', updatePercentage);

  // Initial call to set the initial percentage
  updatePercentage();
</script>

</body>
</html>

Hours spent on the bike: 0

Total kilometers:

Total elevation gain:

Ascents with road bike:

Ascents with blue bike: