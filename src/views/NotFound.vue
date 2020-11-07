<template>
    <div>
        <!-- CONTENIDO PARA LA VISTA DE RUTAS INEXISTENTES -->
        <div class="jumbotron text-center py-3">
            <h1 class="display-5">La pagina que busca no existe</h1>
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

<style scoped>
    .jumbotron{
        background-image: url('../../public/assets/img/chevrolet-blazer.jpg');
        background-size: cover;
        background-position-y: 10%;
        color: white;
        text-shadow: 1px 1px black;
    }
</style>