<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport"
        content="width=device-width, initial-scale=1.0">

  <title>Encantadia Video Editor</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #100d19;
      color: white;
    }

    header {
      padding: 20px;
      text-align: center;
      background: #21162e;
      border-bottom: 1px solid #604478;
    }

    header h1 {
      margin: 0;
      color: #e5c4ff;
      font-size: 25px;
    }

    header p {
      color: #c8bdd6;
      font-size: 13px;
    }

    main {
      max-width: 850px;
      margin: auto;
      padding: 16px;
    }

    .panel {
      background: #1d1727;
      border: 1px solid #493557;
      border-radius: 14px;
      padding: 16px;
      margin-bottom: 18px;
    }

    h2 {
      font-size: 17px;
      color: #e5c4ff;
    }

    .preview {
      width: 100%;
      aspect-ratio: 16 / 9;
      background: black;
      border-radius: 10px;
      overflow: hidden;
      position: relative;
    }

    video {
      width: 100%;
      height: 100%;
      object-fit: contain;
    }

    .gem {
      position: absolute;
      width: 90px;
      height: 90px;
      object-fit: contain;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      pointer-events: none;
      display: none;
    }

    .buttons {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 10px;
    }

    button, .upload {
      background: #382448;
      color: white;
      border: 1px solid #8057a1;
      padding: 13px;
      border-radius: 9px;
      cursor: pointer;
      text-align: center;
      font-size: 14px;
    }

    button:hover, .upload:hover {
      background: #58346e;
    }

    input, select {
      max-width: 100%;
      margin-top: 8px;
      margin-bottom: 12px;
    }

    label {
      display: block;
      margin-top: 14px;
      font-size: 14px;
    }

    .upload {
      display: block;
      margin-top: 10px;
    }

    .upload input {
      display: none;
    }

    .status {
      color: #d5c2e6;
      font-size: 13px;
      overflow-wrap: anywhere;
    }
  </style>
</head>

<body>

<header>
  <h1>💎 ENCANTADIA</h1>
  <p>MAGICAL VIDEO EDITOR</p>
</header>

<main>

  <section class="panel">
    <h2>Video Preview</h2>

    <div class="preview">
      <video id="video" controls playsinline></video>
      <img id="gem" class="gem" alt="Selected gemstone">
    </div>

    <label class="upload">
      📁 Import Your Video
      <input id="videoFile" type="file"
             accept="video/*">
    </label>

    <p class="status" id="status">
      Import a video to begin.
    </p>
  </section>

  <section class="panel">
    <h2>Choose Your Brilyante</h2>

    <div class="buttons">
      <button data-gem="lupa">🌍 Brilyante ng Lupa</button>
      <button data-gem="hangin">🌪️ Brilyante ng Hangin</button>
      <button data-gem="tubig">🌊 Brilyante ng Tubig</button>
      <button data-gem="apoy">🔥 Brilyante ng Apoy</button>
    </div>

    <label class="upload">
      💎 Import Gemstone Video or Image
      <input id="gemFile" type="file"
             accept="video/*,image/*">
    </label>

    <label for="size">Gemstone Size</label>
    <input id="size" type="range"
           min="30" max="250" value="90">

    <label for="animation">Animation</label>
    <select id="animation">
      <option value="none">None</option>
      <option value="fade">Fade In / Fade Out</option>
      <option value="zoom">Zoom In</option>
      <option value="rotate">Rotate</option>
    </select>

    <button id="apply">Apply Animation</button>
    <button id="remove">Remove Gemstone</button>
  </section>

</main>

<script>
  const video = document.getElementById("video");
  const gem = document.getElementById("gem");
  const videoFile = document.getElementById("videoFile");
  const gemFile = document.getElementById("gemFile");
  const size = document.getElementById("size");
  const animation = document.getElementById("animation");
  const status = document.getElementById("status");

  let videoURL = null;
  let gemURL = null;

  videoFile.addEventListener("change", () => {
    const file = videoFile.files[0];
    if (!file) return;

    if (videoURL) URL.revokeObjectURL(videoURL);

    videoURL = URL.createObjectURL(file);
    video.src = videoURL;
    status.textContent = "Video loaded: " + file.name;
  });

  gemFile.addEventListener("change", () => {
    const file = gemFile.files[0];
    if (!file) return;

    if (gemURL) URL.revokeObjectURL(gemURL);

    gemURL = URL.createObjectURL(file);
    gem.src = gemURL;
    gem.style.display = "block";

    status.textContent =
      "Gemstone loaded: " + file.name;
  });

  document.querySelectorAll("[data-gem]").forEach(button => {
    button.addEventListener("click", () => {
      status.textContent =
        "Selected: Brilyante ng " +
        button.dataset.gem.toUpperCase() +
        ". Import its gemstone file to display it.";

      gem.style.display = gemURL ? "block" : "none";
    });
  });

  size.addEventListener("input", () => {
    gem.style.width = size.value + "px";
    gem.style.height = size.value + "px";
  });

  document.getElementById("apply").addEventListener("click", () => {
    gem.style.animation = "none";

    const effect = animation.value;

    if (effect === "fade") {
      gem.style.animation = "fadeGem 2s ease-in-out infinite alternate";
    } else if (effect === "zoom") {
      gem.style.animation = "zoomGem 2s ease-in-out infinite alternate";
    } else if (effect === "rotate") {
      gem.style.animation = "rotateGem 3s linear infinite";
    }
  });

  document.getElementById("remove").addEventListener("click", () => {
    gem.style.display = "none";
    gem.style.animation = "none";
    status.textContent = "Gemstone removed from preview.";
  });
</script>

<style>
  @keyframes fadeGem {
    from { opacity: 0.2; }
    to { opacity: 1; }
  }

  @keyframes zoomGem {
    from {
      transform: translate(-50%, -50%) scale(0.7);
    }
    to {
      transform: translate(-50%, -50%) scale(1.3);
    }
  }

  @keyframes rotateGem {
    from {
      transform: translate(-50%, -50%) rotate(0deg);
    }
    to {
      transform: translate(-50%, -50%) rotate(360deg);
    }
  }
</style>

</body>
</html>
