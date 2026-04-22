---
title: Chimères : le casino dont on ne revient jamais
subtitle: My first post on my new blog
categories: [Books]
---
<div class="lang-switcher">
  <button onclick="showLang('en')" id="btn-en" class="lang-btn active">English</button>
  <button onclick="showLang('fr')" id="btn-fr" class="lang-btn">Français</button>
  <button onclick="showLang('ar')" id="btn-ar" class="lang-btn">العربية</button>
</div>

<div id="lang-en" class="lang-content">

Your **English** content goes here.

Lorem ipsum in English...

</div>

<div id="lang-fr" class="lang-content" style="display:none">

Votre contenu en **français** ici.

Lorem ipsum en français...

</div>

<div id="lang-ar" class="lang-content" style="display:none; direction:rtl; text-align:right">

المحتوى **العربي** هنا.

لوريم إيبسوم بالعربية...

</div>

<script>
function showLang(lang) {
  document.querySelectorAll('.lang-content').forEach(el => el.style.display = 'none');
  document.querySelectorAll('.lang-btn').forEach(btn => btn.classList.remove('active'));
  document.getElementById('lang-' + lang).style.display = 'block';
  document.getElementById('btn-' + lang).classList.add('active');
}
</script>

<style>
.lang-switcher { margin-bottom: 20px; }
.lang-btn {
  padding: 6px 16px;
  margin-right: 6px;
  border: 1px solid #ccc;
  background: white;
  cursor: pointer;
  border-radius: 4px;
}
.lang-btn.active {
  background: #333;
  color: white;
  border-color: #333;
}
</style>
