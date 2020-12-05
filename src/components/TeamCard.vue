<template>
    <div class="integrante" id="contenedor">
        <div class="col aling-items-center">

            <div class="row align-items-center">
                <img :src="require(`@/assets/${member.image}`)" width="100" height="100" alt="" class="imagenIntegrante rounded-circle" >
                <h4 class="ml-2">{{member.nombre}}</h4> <br>
            </div>
                <div class=" align-items-center">
         
                {{member.descripcion}}
                </div>
                <br>
                <div class="especialidad align-baseline">
                    <p> {{member.rol}} </p>
                    <p>Código: {{member.codigo}}</p>    
                </div>
                
                   

        </div>
        
    </div> 
     
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member'],
        
        
        
    }
</script>

<style scoped>



</style>
