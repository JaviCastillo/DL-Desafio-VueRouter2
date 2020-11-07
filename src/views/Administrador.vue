<template>
    <div>
        <!-- CONTENIDO PARA LA VISTA DE 'SOBRE MÍ' -->
        <div class="jumbotron text-center py-3">
            <h1 class="display-3" v-text="tituloEntrada"></h1>
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
    name: 'Administrador',

    computed: {
        tituloEntrada(){
            if(this.$route.params.entrada == 'simple'){
                return 'Bienvenido a la página de Administración'
            }else if(this.$route.params.entrada == 'avanzado'){
                return 'Esta página de administración está en construcción. Intente como administrador simple'
            }else{
                return 'Esta página no existe. Intente como administrador simple'
            }

        },  
    }
}
</script>

<style scoped>
    .jumbotron{
        background-image: url('../../public/assets/img/about-bg.jpg');
        background-size: cover;
        background-position-y: 40%;
        color: white;
        text-shadow: 1px 1px black;
    }
</style>