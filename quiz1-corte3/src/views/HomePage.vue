<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Blank</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <ion-list>
          <inputComponent id="nombre" name="nombre" label="Nombre" fill="outline"/>
          <inputComponent id="fecha-nacimiento" name="fecha-nacimiento" label="Fecha nacimiento" fill="outline"/>
          <inputComponent id="celular" name="celular" label="Celular" fill="outline"/>
          <inputComponent id="correo" name="correo" label="Correo" fill="outline"/>
        </ion-list>
        <buttonComponent id="agregar" value="Agregar"/>
        <buttonComponent id="buscar" value="Buscar" color="success"/>
        <buttonComponent id="modificar" value="Modificar" color="warning"/>
        <buttonComponent id="eliminar" value="Eliminar" color="danger"/>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import buttonComponent from '@/components/buttonComponent.vue';
import inputComponent from '@/components/inputComponent.vue';
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
