
<template>
  <div>
  <hola-mundo-comp></hola-mundo-comp>
  <lista-foros></lista-foros>
  <h1> Dar de alta Foro </h1>
  <form-foro></form-foro>
  <h2> Dar de alta Tema en el Foro </h2>
  <Form-Subject></Form-Subject>
  <Lista-Subject></Lista-Subject>
  </div>
</template>

<script>
import HolaMundoComp from "../components/HolaMundoComp";
import ListaForos from "../components/ListaForos";
import FormForo from "../components/FormForo";
import FormSubject from "../components/FormSubject";
import ListaSubject from "../components/ListaSubject";



export default {
  name: "InicioView",
  components: { HolaMundoComp, ListaForos, FormForo, FormSubject, ListaSubject },
    
};
</script>

<style scoped></style>

