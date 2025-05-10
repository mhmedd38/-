<!DOCTYPE html><html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ترندك - Trendak</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Arial', sans-serif;
      background: #000;
      color: #fff;
      overflow: hidden;
    }
    header {
      text-align: center;
      padding: 1rem;
      background: #111;
      font-size: 1.5rem;
      font-weight: bold;
    }
    .video-feed {
      position: absolute;
      top: 60px;
      bottom: 0;
      width: 100%;
      overflow-y: scroll;
      scroll-snap-type: y mandatory;
    }
    .video-card {
      position: relative;
      scroll-snap-align: start;
      height: 100vh;
      background: #000;
    }
    video {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
    .actions {
      position: absolute;
      right: 10px;
      bottom: 100px;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    .actions button {
      background: rgba(255,255,255,0.1);
      border: none;
      color: #fff;
      padding: 10px;
      border-radius: 10px;
      cursor: pointer;
    }
    .desc {
      position: absolute;
      bottom: 20px;
      left: 10px;
      right: 80px;
      font-size: 1rem;
    }
  </style>
</head>
<body>
  <header>ترندك - Trendak</header>
  <div class="video-feed" id="feed">
    <div class="video-card">
      <video src="https://www.w3schools.com/html/mov_bbb.mp4" autoplay loop muted></video>
      <div class="actions">
        <button>لايك</button>
        <button>تعليق</button>
        <button>مشاركة</button>
      </div>
      <div class="desc">فيديو تجريبي - ترندك</div>
    </div>
    <div class="video-card">
      <video src="https://www.w3schools.com/html/movie.mp4" autoplay loop muted></video>
      <div class="actions">
        <button>لايك</button>
        <button>تعليق</button>
        <button>مشاركة</button>
      </div>
      <div class="desc">فيديو ثاني - ترندك</div>
    </div>
  </div>
</body>
</html>
