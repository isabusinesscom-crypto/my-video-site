<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ad-unlock Video</title>
  <link rel="stylesheet" href="static/css/style.css">
</head>
<body>
  <main>
    <section id="unlock-area" aria-live="polite">
      <p>Ads watched: <span id="count">0</span> / <span id="required">3</span></p>
      <button id="watch-btn">Watch Ad</button>
      <button id="reset-btn" class="muted">Reset</button>
    </section>

    <section id="video-area" style="display:none;">
      <h3>Unlocked!</h3>
      <video controls width="350">
        <source src="your_video_url.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </section>

    <!-- Ad overlay (created/controlled by JS) -->
    <div id="ad-overlay" class="hidden" role="dialog" aria-modal="true" aria-label="Advertisement">
      <div class="ad-content">
        <p id="ad-text">Ad — please watch</p>
        <p id="ad-countdown" aria-live="polite"></p>
      </div>
    </div>
  </main>

  <script src="static/js/app.js"></script>
</body>
</html>
