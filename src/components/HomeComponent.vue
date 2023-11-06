<template>
    <div>
        <h1 style="color:red">
            Proyecto Servicios VUE
        </h1>
    </div>
</template>

<script>
import ServiceEjemplo from '../services/ServiceEjemplo';

const service = new ServiceEjemplo();

    export default {
        name: "HomeComponent",
        mounted(){
            this.mensaje = service.getSaludo("alumno");
        },
        data(){
            return {
                mensaje : ""
            }
        }
    }
</script>