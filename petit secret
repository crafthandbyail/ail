<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>lesyeuxdenini</title>

<style>
:root {
  --bg: #fff;
  --text: #080808;
  --button: #f0eff4;
  --border: #dedede;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  background: var(--bg);
  color: var(--text);
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
}

button, input, textarea {
  font: inherit;
}

button {
  cursor: pointer;
}

.app {
  max-width: 850px;
  min-height: 100vh;
  margin: auto;
  background: white;
}

/* HEADER */

.header {
  height: 110px;
  padding: 0 25px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
}

.icon-button {
  width: 42px;
  height: 45px;
  padding: 0;
  flex-shrink: 0;
  border: none;
  background: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
}

.icon-button svg {
  width: 35px;
  height: 35px;
  fill: none;
  stroke: currentColor;
  stroke-width: 2;
  stroke-linecap: round;
}

.username-heading {
  flex: 1;
  min-width: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 12px;
}

.username-heading h1 {
  margin: 0;
  font-size: clamp(22px, 5.3vw, 42px);
  font-weight: 750;
  letter-spacing: -1.5px;
  text-align: center;
  overflow-wrap: anywhere;
}

.dropdown-arrow {
  width: 13px;
  height: 13px;
  border-right: 2px solid;
  border-bottom: 2px solid;
  transform: rotate(45deg) translateY(-3px);
  flex-shrink: 0;
}

/* PROFILE */

.profile {
  padding: 55px 35px 40px;
}

.profile-top {
  margin-bottom: 45px;
}

.avatar {
  width: 205px;
  height: 205px;
  padding: 0;
  border: none;
  border-radius: 50%;
  overflow: hidden;
  background: #f0eff4;
  display: flex;
  align-items: center;
  justify-content: center;
}

.avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.avatar-placeholder {
  font-size: 46px;
  color: #888;
}

.profile-name {
  margin: 0 0 15px;
  font-size: 34px;
  line-height: 1.2;
  font-weight: 750;
  overflow-wrap: anywhere;
}

.bio {
  margin: 0;
  font-size: 28px;
  line-height: 1.4;
  white-space: pre-wrap;
  overflow-wrap: anywhere;
}

/* MINI SPOTIFY */

.music-section {
  margin-top: 18px;
  margin-bottom: 35px;
  width: 100%;
}

.music-section:empty {
  display: none;
}

.spotify-frame {
  display: block;
  width: 100%;
  max-width: 440px;
  height: 80px;
  border: none;
  border-radius: 14px;
  background: #0b0d12;
}

.spotify-frame.playlist,
.spotify-frame.album,
.spotify-frame.show {
  height: 152px;
}

.music-error {
  font-size: 13px;
  color: #777;
}

/* ACTION BUTTONS */

.actions {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 1fr) 90px;
  gap: 12px;
  margin-bottom: 65px;
}

.action-button {
  min-height: 78px;
  padding: 12px;
  border: none;
  border-radius: 26px;
  background: var(--button);
  color: #080808;
  font-size: 23px;
  font-weight: 650;
}

.action-button:hover {
  background: #e7e6eb;
}

.action-button svg {
  width: 35px;
  height: 35px;
  fill: none;
  stroke: currentColor;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
}

/* HIGHLIGHTS */

.highlights {
  display: flex;
  align-items: flex-start;
  gap: 28px;
  flex-wrap: wrap;
}

.highlight {
  width: 170px;
  color: var(--text);
  text-decoration: none;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 15px;
  overflow-wrap: anywhere;
}

.highlight-circle {
  width: 170px;
  height: 170px;
  padding: 11px;
  border: 5px solid #dedede;
  border-radius: 50%;
}

.highlight-inner {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: var(--button);
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

.highlight-inner img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.highlight-inner svg {
  width: 45px;
  height: 45px;
  fill: none;
  stroke: #080808;
  stroke-width: 2.5;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.highlight-label {
  font-size: 20px;
  line-height: 1.3;
}

.empty-highlights {
  color: #888;
  font-size: 14px;
}

/* EDITOR */

.modal-overlay {
  position: fixed;
  inset: 0;
  z-index: 100;
  background: rgba(0,0,0,.4);
  display: none;
  align-items: center;
  justify-content: center;
  padding: 15px;
}

.modal-overlay.open {
  display: flex;
}

.modal {
  width: 100%;
  max-width: 520px;
  max-height: 90vh;
  overflow-y: auto;
  padding: 25px;
  border-radius: 22px;
  background: white;
}

.modal-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  margin-bottom: 25px;
}

.modal-header h2 {
  margin: 0;
  font-size: 23px;
}

.close-button {
  padding: 5px;
  border: none;
  background: transparent;
  font-size: 28px;
}

.form-group {
  margin-bottom: 19px;
}

.form-group label {
  display: block;
  margin-bottom: 8px;
  font-size: 14px;
  font-weight: 650;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 13px 14px;
  border: 1px solid #dedede;
  border-radius: 12px;
  background: #fafafa;
  color: #111;
}

.form-group textarea {
  min-height: 95px;
  resize: vertical;
}

.form-help,
.notice {
  display: block;
  margin-top: 7px;
  color: #777;
  font-size: 12px;
  line-height: 1.6;
}

.avatar-preview {
  display: block;
  width: 90px;
  height: 90px;
  margin-bottom: 12px;
  border-radius: 50%;
  object-fit: cover;
  background: #f0eff4;
}

.divider {
  height: 1px;
  margin: 25px 0;
  background: #eee;
}

.editor-highlight {
  padding: 15px;
  margin-bottom: 12px;
  border: 1px solid #e5e5e5;
  border-radius: 14px;
}

.editor-highlight h4 {
  margin: 0 0 13px;
  font-size: 15px;
}

.editor-highlight .form-group {
  margin-bottom: 12px;
}

.delete-button {
  padding: 9px 12px;
  margin-top: 12px;
  border: none;
  border-radius: 9px;
  background: #f5eaea;
  color: #a33131;
  font-size: 13px;
}

.add-button,
.reset-button {
  width: 100%;
  padding: 13px;
  border: 1px solid #ddd;
  border-radius: 12px;
  background: white;
}

.add-button {
  border-style: dashed;
}

.save-button {
  width: 100%;
  padding: 16px;
  margin-top: 15px;
  border: none;
  border-radius: 14px;
  background: #080808;
  color: white;
  font-weight: 650;
}

.reset-button {
  margin-top: 10px;
  color: #666;
}

.share-link {
  display: flex;
  gap: 8px;
}

.share-link input {
  min-width: 0;
  flex: 1;
  padding: 12px;
  border: 1px solid #ddd;
  border-radius: 10px;
}

.share-link button {
  padding: 12px;
  border: none;
  border-radius: 10px;
  background: #080808;
  color: white;
}

.toast {
  position: fixed;
  bottom: 25px;
  left: 50%;
  z-index: 200;
  max-width: 90%;
  padding: 13px 20px;
  border-radius: 12px;
  background: #111;
  color: white;
  font-size: 14px;
  text-align: center;
  opacity: 0;
  pointer-events: none;
  transform: translateX(-50%);
  transition: opacity .2s;
}

.toast.show {
  opacity: 1;
}

@media (max-width: 600px) {
  .header {
    height: 105px;
    padding: 0 22px;
  }

  .icon-button {
    width: 38px;
  }

  .icon-button svg {
    width: 31px;
    height: 31px;
  }

  .username-heading {
    gap: 10px;
  }

  .username-heading h1 {
    letter-spacing: -1px;
  }

  .profile {
    padding: 42px 4% 35px;
  }

  .profile-top {
    margin-bottom: 42px;
  }

  .avatar {
    width: 155px;
    height: 155px;
  }

  .profile-name {
    font-size: 30px;
    margin-bottom: 13px;
  }

  .bio {
    font-size: 25px;
    line-height: 1.45;
  }

  .spotify-frame {
    max-width: 100%;
    height: 80px;
  }

  .spotify-frame.playlist,
  .spotify-frame.album,
  .spotify-frame.show {
    height: 152px;
  }

  .actions {
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr) 68px;
    gap: 10px;
    margin-bottom: 60px;
  }

  .action-button {
    min-height: 70px;
    padding: 8px;
    border-radius: 23px;
    font-size: clamp(15px, 4.2vw, 22px);
  }

  .action-button svg {
    width: 30px;
    height: 30px;
  }

  .highlights {
    gap: 20px;
  }

  .highlight {
    width: 125px;
  }

  .highlight-circle {
    width: 125px;
    height: 125px;
    padding: 9px;
    border-width: 5px;
  }

  .highlight-inner svg {
    width: 36px;
    height: 36px;
  }

  .highlight-label {
    font-size: 18px;
  }
}

@media (max-width: 370px) {
  .header {
    padding: 0 12px;
  }

  .username-heading h1 {
    font-size: 22px;
  }

  .profile {
    padding-right: 15px;
    padding-left: 15px;
  }

  .actions {
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr) 55px;
    gap: 6px;
  }

  .action-button {
    font-size: 14px;
  }

  .highlight {
    width: 110px;
  }

  .highlight-circle {
    width: 110px;
    height: 110px;
  }
}
</style>
</head>

<body>
<main class="app">

  <header class="header">

    <button class="icon-button" id="addButton"
      aria-label="Edit profile">
      <svg viewBox="0 0 40 40">
        <path d="M20 5 V35 M5 20 H35"/>
      </svg>
    </button>

    <div class="username-heading">
      <h1 id="usernameHeading">lesyeuxdenini</h1>
      <span class="dropdown-arrow"></span>
    </div>

    <button class="icon-button" id="menuButton"
      aria-label="Open settings">
      <svg viewBox="0 0 40 40">
        <path d="M5 9 H35 M5 20 H35 M5 31 H35"/>
      </svg>
    </button>

  </header>

  <section class="profile">

    <div class="profile-top">
      <button class="avatar" id="avatarButton"
        aria-label="Edit profile picture">
        <img id="profileAvatar" alt="Profile picture"
          style="display:none">
        <span class="avatar-placeholder" id="avatarPlaceholder">+</span>
      </button>
    </div>

    <div class="profile-information">
      <h2 class="profile-name" id="displayName">jemappelle</h2>
      <p class="bio" id="displayBio">i hope you read it—until the end???</p>
    </div>

    <!-- MINI SPOTIFY PLAYER UNDER BIO -->
    <section class="music-section" id="musicSection"></section>

    <div class="actions">

      <button class="action-button" id="followButton">
        Follow
      </button>

      <button class="action-button" id="shareButton">
        Share profile
      </button>

      <button class="action-button" id="quickEditButton"
        aria-label="Edit profile">
        <svg viewBox="0 0 40 40">
          <circle cx="14" cy="12" r="7"/>
          <path d="M2 34 C2 25 8 21 16 21 C20 21 23 22 26 25"/>
          <path d="M30 22 V36 M23 29 H37"/>
        </svg>
      </button>

    </div>

    <section class="highlights" id="highlights"></section>

  </section>
</main>

<!-- EDIT PROFILE -->

<div class="modal-overlay" id="editorOverlay"
  role="dialog" aria-modal="true" aria-labelledby="editorTitle">

  <div class="modal">

    <div class="modal-header">
      <h2 id="editorTitle">Edit profile</h2>
      <button class="close-button" id="closeEditor"
        aria-label="Close">&times;</button>
    </div>

    <form id="profileForm">

      <div class="form-group">
        <label for="inputUsername">Username</label>
        <input id="inputUsername" maxlength="40"
          placeholder="lesyeuxdenini" required>
      </div>

      <div class="form-group">
        <label for="inputName">Name</label>
        <input id="inputName" maxlength="100"
          placeholder="jemappelle">
      </div>

      <div class="form-group">
        <label for="inputBio">Bio</label>
        <textarea id="inputBio" maxlength="500"
          placeholder="i hope you read it—until the end???"></textarea>
      </div>

      <div class="divider"></div>

      <div class="form-group">
        <label for="inputAvatar">Profile picture</label>
        <img id="avatarPreview" class="avatar-preview"
          alt="Avatar preview" style="display:none">

        <input id="inputAvatar" type="file" accept="image/*">

        <span class="form-help">
          Choose an image up to 3 MB. Square images work best.
        </span>

        <button type="button" class="delete-button"
          id="removeAvatar">Remove profile picture</button>
      </div>

      <div class="divider"></div>

      <div class="form-group">
        <label for="inputSpotify">Spotify song or playlist link</label>
        <input id="inputSpotify" type="url"
          placeholder="https://open.spotify.com/track/...">

        <span class="form-help">
          Paste a Spotify track, playlist, or album link.
          The mini player will appear underneath your bio.
        </span>
      </div>

      <div class="divider"></div>

      <div class="form-group">
        <label>Highlights / Links</label>
        <span class="form-help">
          Add links to your websites, social media, or other pages.
        </span>
      </div>

      <div id="highlightEditor"></div>

      <button type="button" class="add-button" id="addHighlight">
        + Add highlight
      </button>

      <p class="notice">
        Your changes are saved in this browser only.
        They won't automatically sync to other devices.
      </p>

      <button type="submit" class="save-button">
        Save changes
      </button>

      <button type="button" class="reset-button" id="resetProfile">
        Reset to original profile
      </button>

    </form>
  </div>
</div>

<!-- SHARE PROFILE -->

<div class="modal-overlay" id="shareOverlay"
  role="dialog" aria-modal="true" aria-labelledby="shareTitle">

  <div class="modal">

    <div class="modal-header">
      <h2 id="shareTitle">Share profile</h2>
      <button class="close-button" id="closeShare"
        aria-label="Close">&times;</button>
    </div>

    <p style="color:#666;line-height:1.6">
      Copy this page's address to share it.
    </p>

    <div class="share-link">
      <input id="shareUrl" type="text" readonly
        aria-label="Profile URL">
      <button type="button" id="copyShare">Copy</button>
    </div>

    <p class="notice">
      Publish your website online before sharing it with others.
    </p>

  </div>
</div>

<div class="toast" id="toast" role="status"></div>

<script>
const DEFAULT_PROFILE = {
  username: "lesyeuxdenini",
  name: "jemappelle",
  bio: "i hope you read it—until the end???",
  avatar: "",
  spotify: "",
  highlights: [
    { title: "hi", url: "", image: "" }
  ]
};

const STORAGE_KEY = "lesyeuxdenini_profile_v2";

const $ = id => document.getElementById(id);

function cloneDefault() {
  return JSON.parse(JSON.stringify(DEFAULT_PROFILE));
}

function loadProfile() {
  try {
    const saved = localStorage.getItem(STORAGE_KEY);

    if (!saved) return cloneDefault();

    const parsed = JSON.parse(saved);

    return {
      ...cloneDefault(),
      ...parsed,
      highlights: Array.isArray(parsed.highlights)
        ? parsed.highlights
        : cloneDefault().highlights
    };
  } catch {
    return cloneDefault();
  }
}

let profile = loadProfile();
let pendingAvatar = profile.avatar || "";

function saveProfile() {
  try {
    localStorage.setItem(STORAGE_KEY, JSON.stringify(profile));
    return true;
  } catch {
    showToast("Storage is full. Try a smaller image.");
    return false;
  }
}

/* RENDER PROFILE */

function renderProfile() {
  $("usernameHeading").textContent = profile.username || "";
  $("displayName").textContent = profile.name || "";
  $("displayBio").textContent = profile.bio || "";

  document.title = (profile.username || "Profile") + " — Profile";

  renderAvatar();
  renderSpotify();
  renderHighlights();
}

function renderAvatar() {
  const img = $("profileAvatar");
  const placeholder = $("avatarPlaceholder");

  if (profile.avatar) {
    img.src = profile.avatar;
    img.style.display = "block";
    placeholder.style.display = "none";
  } else {
    img.removeAttribute("src");
    img.style.display = "none";
    placeholder.style.display = "block";
  }
}

/* SPOTIFY URL */

function getSpotifyEmbedUrl(input) {
  if (!input) return "";

  try {
    const url = new URL(input.trim());
    const host = url.hostname.toLowerCase();

    if (host !== "open.spotify.com") return "";

    const parts = url.pathname.split("/").filter(Boolean);
    const type = parts[0];
    const id = parts[1];

    const supported = [
      "track", "playlist", "album", "episode", "show"
    ];

    if (!supported.includes(type) || !id) return "";
    if (!/^[a-zA-Z0-9]+$/.test(id)) return "";

    return "https://open.spotify.com/embed/" +
      type + "/" + id + "?utm_source=generator";

  } catch {
    return "";
  }
}

/* MINI SPOTIFY PLAYER */

function renderSpotify() {
  const section = $("musicSection");
  section.replaceChildren();

  if (!profile.spotify) return;

  const embedUrl = getSpotifyEmbedUrl(profile.spotify);

  if (!embedUrl) {
    const message = document.createElement("p");
    message.className = "music-error";
    message.textContent =
      "Please enter a valid Spotify track, playlist, or album link.";

    section.appendChild(message);
    return;
  }

  const iframe = document.createElement("iframe");

  iframe.className = "spotify-frame";

  if (embedUrl.includes("/embed/playlist/")) {
    iframe.classList.add("playlist");
  } else if (embedUrl.includes("/embed/album/")) {
    iframe.classList.add("album");
  } else if (embedUrl.includes("/embed/show/")) {
    iframe.classList.add("show");
  }

  iframe.src = embedUrl;
  iframe.title = "Spotify music player";
  iframe.loading = "lazy";

  iframe.setAttribute(
    "allow",
    "autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
  );

  iframe.setAttribute("allowfullscreen", "");
  iframe.referrerPolicy = "strict-origin-when-cross-origin";

  section.appendChild(iframe);
}

/* HIGHLIGHTS */

function validateWebUrl(value) {
  if (!value) return "";

  try {
    const url = new URL(value.trim());

    if (!["https:", "http:"].includes(url.protocol)) return "";

    return url.href;
  } catch {
    return "";
  }
}

function createLinkIcon() {
  const svg = document.createElementNS(
    "http://www.w3.org/2000/svg", "svg"
  );

  svg.setAttribute("viewBox", "0 0 48 48");

  const path = document.createElementNS(
    "http://www.w3.org/2000/svg", "path"
  );

  path.setAttribute(
    "d",
    "M19 29l-3 3a8 8 0 0 1-11-11l8-8a8 8 0 0 1 11 0 M29 19l3-3a8 8 0 0 1 11 11l-8 8a8 8 0 0 1-11 0 M17 31l14-14"
  );

  svg.appendChild(path);
  return svg;
}

function renderHighlights() {
  const container = $("highlights");
  container.replaceChildren();

  if (!profile.highlights.length) {
    const empty = document.createElement("p");
    empty.className = "empty-highlights";
    empty.textContent = "No highlights yet.";
    container.appendChild(empty);
    return;
  }

  profile.highlights.forEach(item => {
    const link = document.createElement("a");
    link.className = "highlight";

    const circle = document.createElement("div");
    circle.className = "highlight-circle";

    const inner = document.createElement("div");
    inner.className = "highlight-inner";

    if (item.image) {
      const img = document.createElement("img");
      img.src = item.image;
      img.alt = "";
      inner.appendChild(img);
    } else {
      inner.appendChild(createLinkIcon());
    }

    circle.appendChild(inner);

    const label = document.createElement("span");
    label.className = "highlight-label";
    label.textContent = item.title || "link";

    link.append(circle, label);

    const url = validateWebUrl(item.url);

    if (url) {
      link.href = url;
      link.target = "_blank";
      link.rel = "noopener noreferrer";
    } else {
      link.href = "#";

      link.addEventListener("click", event => {
        event.preventDefault();

        if (!item.url) {
          showToast("Add a link in Edit profile first.");
        }
      });
    }

    container.appendChild(link);
  });
}

/* EDITOR */

function openEditor() {
  $("inputUsername").value = profile.username || "";
  $("inputName").value = profile.name || "";
  $("inputBio").value = profile.bio || "";
  $("inputSpotify").value = profile.spotify || "";

  pendingAvatar = profile.avatar || "";
  $("inputAvatar").value = "";

  if (pendingAvatar) {
    $("avatarPreview").src = pendingAvatar;
    $("avatarPreview").style.display = "block";
  } else {
    $("avatarPreview").removeAttribute("src");
    $("avatarPreview").style.display = "none";
  }

  renderHighlightEditor();

  $("editorOverlay").classList.add("open");
  document.body.style.overflow = "hidden";
}

function closeEditor() {
  $("editorOverlay").classList.remove("open");
  document.body.style.overflow = "";
}

$("addButton").addEventListener("click", openEditor);
$("menuButton").addEventListener("click", openEditor);
$("quickEditButton").addEventListener("click", openEditor);
$("avatarButton").addEventListener("click", openEditor);
$("closeEditor").addEventListener("click", closeEditor);

$("editorOverlay").addEventListener("click", event => {
  if (event.target === $("editorOverlay")) closeEditor();
});

/* AVATAR UPLOAD */

$("inputAvatar").addEventListener("change", function() {
  const file = this.files && this.files[0];

  if (!file) return;

  if (!file.type.startsWith("image/")) {
    showToast("Please choose an image file.");
    this.value = "";
    return;
  }

  if (file.size > 3 * 1024 * 1024) {
    showToast("Choose an image under 3 MB.");
    this.value = "";
    return;
  }

  const reader = new FileReader();

  reader.onload = event => {
    pendingAvatar = event.target.result;
    $("avatarPreview").src = pendingAvatar;
    $("avatarPreview").style.display = "block";
  };

  reader.readAsDataURL(file);
});

$("removeAvatar").addEventListener("click", () => {
  pendingAvatar = "";
  $("inputAvatar").value = "";
  $("avatarPreview").removeAttribute("src");
  $("avatarPreview").style.display = "none";
});

/* HIGHLIGHT EDITOR */

function syncHighlightFields() {
  const cards = Array.from($("highlightEditor").children);

  profile.highlights = cards.map((card, index) => {
    const old = profile.highlights[index] || {};

    return {
      title: card.querySelector(".highlight-title").value.trim(),
      url: card.querySelector(".highlight-url").value.trim(),
      image: old.image || ""
    };
  });
}

function renderHighlightEditor() {
  const editor = $("highlightEditor");
  editor.replaceChildren();

  profile.highlights.forEach((item, index) => {
    const card = document.createElement("div");
    card.className = "editor-highlight";

    const heading = document.createElement("h4");
    heading.textContent = "Highlight " + (index + 1);

    const titleGroup = document.createElement("div");
    titleGroup.className = "form-group";

    const titleLabel = document.createElement("label");
    titleLabel.textContent = "Title";

    const titleInput = document.createElement("input");
    titleInput.className = "highlight-title";
    titleInput.type = "text";
    titleInput.maxLength = 50;
    titleInput.placeholder = "hi";
    titleInput.value = item.title || "";

    titleLabel.appendChild(titleInput);
    titleGroup.appendChild(titleLabel);

    const urlGroup = document.createElement("div");
    urlGroup.className = "form-group";

    const urlLabel = document.createElement("label");
    urlLabel.textContent = "Link URL";

    const urlInput = document.createElement("input");
    urlInput.className = "highlight-url";
    urlInput.type = "url";
    urlInput.placeholder = "https://example.com";
    urlInput.value = item.url || "";

    urlLabel.appendChild(urlInput);
    urlGroup.appendChild(urlLabel);

    const imageGroup = document.createElement("div");
    imageGroup.className = "form-group";

    const imageLabel = document.createElement("label");
    imageLabel.textContent = "Highlight cover (optional)";

    const imageInput = document.createElement("input");
    imageInput.type = "file";
    imageInput.accept = "image/*";

    imageLabel.appendChild(imageInput);
    imageGroup.appendChild(imageLabel);

    const help = document.createElement("span");
    help.className = "form-help";
    help.textContent = "Optional image for your highlight.";

    imageGroup.appendChild(help);

    imageInput.addEventListener("change", function() {
      const file = this.files && this.files[0];

      if (!file) return;

      if (!file.type.startsWith("image/") ||
          file.size > 3 * 1024 * 1024) {
        showToast("Choose an image under 3 MB.");
        this.value = "";
        return;
      }

      const reader = new FileReader();

      reader.onload = event => {
        item.image = event.target.result;
        showToast("Cover selected. Save changes to apply.");
      };

      reader.readAsDataURL(file);
    });

    const remove = document.createElement("button");
    remove.type = "button";
    remove.className = "delete-button";
    remove.textContent = "Remove highlight";

    remove.addEventListener("click", () => {
      syncHighlightFields();
      profile.highlights.splice(index, 1);
      renderHighlightEditor();
    });

    card.append(
      heading,
      titleGroup,
      urlGroup,
      imageGroup,
      remove
    );

    editor.appendChild(card);
  });
}

$("addHighlight").addEventListener("click", () => {
  syncHighlightFields();

  if (profile.highlights.length >= 20) {
    showToast("You can add up to 20 highlights.");
    return;
  }

  profile.highlights.push({
    title: "",
    url: "",
    image: ""
  });

  renderHighlightEditor();
});

/* SAVE CHANGES */

$("profileForm").addEventListener("submit", event => {
  event.preventDefault();

  const username = $("inputUsername").value.trim();

  if (!username) {
    showToast("Please enter a username.");
    return;
  }

  syncHighlightFields();

  const highlights = [];

  for (const item of profile.highlights) {
    const title = (item.title || "").trim();
    const url = (item.url || "").trim();

    if (!title && !url && !item.image) continue;

    if (url && !validateWebUrl(url)) {
      showToast("Please enter a valid HTTP or HTTPS link.");
      return;
    }

    highlights.push({
      title: title || "link",
      url,
      image: item.image || ""
    });
  }

  const spotify = $("inputSpotify").value.trim();

  if (spotify && !getSpotifyEmbedUrl(spotify)) {
    showToast("Please enter a valid Spotify track or playlist link.");
    return;
  }

  profile.username = username.replace(/^@+/, "");
  profile.name = $("inputName").value.trim();
  profile.bio = $("inputBio").value;
  profile.avatar = pendingAvatar;
  profile.spotify = spotify;
  profile.highlights = highlights;

  if (saveProfile()) {
    renderProfile();
    closeEditor();
    showToast("Profile saved successfully!");
  }
});

/* RESET PROFILE */

$("resetProfile").addEventListener("click", () => {
  if (!confirm("Reset your profile to its original settings?")) return;

  profile = cloneDefault();
  pendingAvatar = "";

  try {
    localStorage.removeItem(STORAGE_KEY);
  } catch {}

  renderProfile();
  closeEditor();
  showToast("Profile reset.");
});

/* SHARE PROFILE */

$("shareButton").addEventListener("click", () => {
  $("shareUrl").value = window.location.href;
  $("shareOverlay").classList.add("open");
});

$("closeShare").addEventListener("click", () => {
  $("shareOverlay").classList.remove("open");
});

$("shareOverlay").addEventListener("click", event => {
  if (event.target === $("shareOverlay")) {
    $("shareOverlay").classList.remove("open");
  }
});

$("copyShare").addEventListener("click", async () => {
  const input = $("shareUrl");

  try {
    await navigator.clipboard.writeText(input.value);
    showToast("Profile link copied!");
  } catch {
    input.select();

    const copied = document.execCommand("copy");

    showToast(copied
      ? "Profile link copied!"
      : "Please copy the link manually.");
  }
});

/* FOLLOW BUTTON */

$("followButton").addEventListener("click", () => {
  showToast("The Follow button is currently a visual element.");
});

/* NOTIFICATIONS */

let toastTimer;

function showToast(message) {
  const toast = $("toast");

  toast.textContent = message;
  toast.classList.add("show");

  clearTimeout(toastTimer);

  toastTimer = setTimeout(() => {
    toast.classList.remove("show");
  }, 2800);
}

document.addEventListener("keydown", event => {
  if (event.key === "Escape") {
    closeEditor();
    $("shareOverlay").classList.remove("open");
  }
});

/* INITIALIZE */

renderProfile();
</script>
</body>
</html>
