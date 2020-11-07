<template>
    <div>
        <!-- CONTENIDO PARA LA VISTA DE PORTADA -->
        <div class="jumbotron text-center py-3">
            <h1 class="display-3">V8</h1>
            <p class="lead">Noticias y reseñas de automóviles</p>
        </div>
        <div class="container">
            <div class="row">
                <div class="col-md-10 col-lg-8">
                    <div class="post-preview">
                        <router-link to="/post/1">
                            <h2 class="post-title"><strong>Chevrolet presenta la totalmente nueva Blazer</strong></h2>
                            <h3 class="post-subtitle">Llega como la primera SUV deportiva de la marca</h3>
                        </router-link>
                    </div>
                    <hr>
                </div>
            </div>
        </div>
        <footer>
            <div class="container fixed-bottom">
                <div class="row">
                    <div class="col-md-10 col-lg-8 mx-auto">
                        <ul class="list-inline text-center">
                            <li class="list-inline-item"><span class="fa-stack fa-lg"><font-awesome-icon :icon="['fas','circle']" size="xs" /><font-awesome-icon :icon="['fab','twitter']" size="2x"/></span></li>
                            <li class="list-inline-item"><span class="fa-stack fa-lg"><font-awesome-icon :icon="['fas','circle']" size="xs" /><font-awesome-icon :icon="['fab','facebook']" size="2x"/></span></li>
                            <li class="list-inline-item"><span class="fa-stack fa-lg"><font-awesome-icon :icon="['fas','circle']" size="xs" /><font-awesome-icon :icon="['fab','github']" size="2x"/></span></li>
                        </ul>
                        <p class="text-muted copyright">Copyright © V8 - 2018</p>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'Portada'
}
</script>

<style scoped>
    .jumbotron{
        background-image: url('../../public/assets/img/home-bg.jpg');
        background-size: cover;
        background-position-y: 30%;
        color: white;
        text-shadow: 1px 1px black;
    }
</style>