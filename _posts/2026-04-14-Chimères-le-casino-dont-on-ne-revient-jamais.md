---
title: "Chimères : le casino dont on ne revient jamais"
subtitle: My first post on my new blog
categories: [Books]
---
<div class="lang-switcher">
  <button onclick="showLang('en')" id="btn-en" class="lang-btn active">English</button>
  <button onclick="showLang('fr')" id="btn-fr" class="lang-btn">Français</button>
  <button onclick="showLang('ar')" id="btn-ar" class="lang-btn">العربية</button>
</div>

<div id="lang-en" class="lang-content">
While I was out with my friend in the old medina , I noticed a bookstore selling unbuyed books for 90% off . <b>"10 Dh each"</b>it said. I picked up 3 books . This was the first one , took me 5 hours to finish , so let's recap and review . 
<b>PS:</b> What sparked my attention (beside the beautiful cover and the book's new condition) were the words "virus informatique" in the blurb .
<img src="https://github.com/user-attachments/assets/a4bba71b-0d91-41b5-82e3-a8e3e3f48493" 
     style="display:block; margin:auto; max-width:100%;" 
     alt="Bookstore">
<h2>Summary</h2>
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
