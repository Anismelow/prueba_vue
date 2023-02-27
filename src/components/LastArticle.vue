<script>
export default {

    name:'LastArticle'
}

window.addEventListener("load", function(){
                        var template = document.getElementById("article-template");
                        var articles = document.getElementById("articles");

                        for(var i = 1; i <= 5; i++){
                            var clonado = template.cloneNode(true);
                            clonado.removeAttribute("id");

                            var h2 = clonado.getElementsByTagName("h2")[0];
                            h2.innerHTML = h2.textContent + ' ' + i;

                            articles.appendChild(clonado);
                        }
        
                    });
                
</script>

<template>
      <section id="content">
                <h2 class="subheader">Últimos artículos</h2>
                
                <!--Listado articulos-->
                <div id="articles">
                    <article class="article-item" id="article-template">
                        <div class="image-wrap">
                            <img src="../assets/image/logo.png" alt="Paisaje" />
                        </div>
    
                        <h2>Articulo de prueba</h2>
                        <span class="date">
                            Hace 5 minutos
                        </span>
                        <a href="#">Leer más</a>

                        <div class="clearfix"></div>
                    </article>

                    <!--AÑADIR ARTICULOS VIA JS-->

                </div>
                
            </section>
</template>