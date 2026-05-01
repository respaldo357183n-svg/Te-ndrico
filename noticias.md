---
title: "Noticias"
layout: archive
permalink: /noticias/
author_profile: false
classes: wide
---
<input type="text" id="buscador" placeholder="Buscar noticias..." onkeyup="filtrar()" style="width:100%;padding:0.8rem 1rem;border:1px solid #e5e5e0;font-size:1rem;margin-bottom:2rem;font-family:'Helvetica Neue',Arial,sans-serif;outline:none;">
<div id="lista-noticias">
{% include archive-list-noticias.html %}
</div>
<script>
function filtrar() {
  var texto = document.getElementById('buscador').value.toLowerCase();
  var noticias = document.querySelectorAll('.article-list-item');
  noticias.forEach(function(noticia) {
    var contenido = noticia.innerText.toLowerCase();
    if (contenido.includes(texto)) {
      noticia.style.display = 'flex';
    } else {
      noticia.style.display = 'none';
    }
  });
}
</script>
