
<template>
  <div>
  <hola-mundo-comp></hola-mundo-comp>
  <lista-foros></lista-foros>
  <h1> Dar de alta Foro </h1>
 <form-foro></form-foro>
  <Lista-Subject></Lista-Subject>
  <h1> Dar de alta Tema en el Foro </h1>
  <Form-Subject></Form-Subject>
  </div>
</template>

<script>
import HolaMundoComp from "../components/HolaMundoComp";
import ListaForos from "../components/ListaForos";
import FormForo from "../components/FormForo";
import ListaSubject from "../components/ListaSubject";
import FormSubject from "../components/FormSubject";




export default {
  name: "InicioView",
  components: { HolaMundoComp, ListaForos, FormForo, ListaSubject, FormSubject },
    
};
</script>

<style scoped></style>

