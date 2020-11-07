<template>
    <div>
        <!-- CONTENIDO PARA LA VISTA DE CONTACTO -->
        <div class="jumbotron text-center py-3">
            <h1 class="display-3">Contacto</h1>
        </div>

        <div class="container">
            <div class="row">
                <div class="col-md-10 col-lg-8 mx-auto">
                    <p>¿Tienes dudas o sugerencias? Déjame un mensaje y me contactaré contigo.<br><br></p>
                    <form id="contactForm" name="sentMessage" novalidate="novalidate">
                        <div class="control-group">
                            <div class="form-group floating-label-form-group controls"><label>Name</label><input class="form-control" type="text" id="name" required="" placeholder="Nombre"><small class="form-text text-danger help-block"></small></div>
                        </div>
                        <div class="control-group">
                            <div class="form-group floating-label-form-group controls"><label>Email Address</label><input class="form-control" type="email" id="email" required="" placeholder="Email "><small class="form-text text-danger help-block"></small></div>
                        </div>
                        <div class="control-group">
                            <div class="form-group floating-label-form-group controls"><label>Phone Number</label><input class="form-control" type="tel" id="phone" required="" placeholder="Teléfono"><small class="form-text text-danger help-block"></small></div>
                        </div>
                        <div class="control-group">
                            <div class="form-group floating-label-form-group controls mb-3"><label>Message</label><textarea class="form-control" id="message" data-validation-required-message="Please enter a message." required="" placeholder="Mensaje" rows="5"></textarea><small class="form-text text-danger help-block"></small></div>
                        </div>
                        <div id="success"></div>
                        <div class="form-group"><button class="btn btn-primary" id="sendMessageButton" type="submit">enviar mensaje</button></div>
                    </form>
                </div>
            </div>
        </div>
        <hr>
        <footer>
            <div class="container">
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
    name: 'Contacto'
}
</script>

<style scoped>
    .jumbotron{
        background-image: url('../../public/assets/img/contact-bg.jpg');
        background-size: contain;
        background-position-y: 10%;
        color: skyblue;
        text-shadow: 2px 2px black;
    }
</style>