<template>
  <div>
    <h1 class="m-5 font-bold text-2xl">Formulario con valores</h1>

    <div class="m-5 font-medium">
      Paterno:
      <input v-model="paterno" class="border border-black" /><br />
      Materno:
      <input v-model="materno" class="border border-black" /><br />
      Nombres:
      <input v-model="nombres" class="border border-black" /><br />
      Sexo:
      <input type="radio" id="hombre" value="Hombre" v-model="sexo" />
      <label for="hombre">Hombre </label>
      <input type="radio" id="mujer" value="Mujer" v-model="sexo" />
      <label for="mujer"> Mujer</label><br />
      Materia:
      <select v-model="materia" class="border border-black">
        <option value="Curso 1">Cálculo</option>
        <option value="Curso 2">Programación</option>
        <option value="Curso 3">Diseño</option>
        <option value="Curso 4">Algoritmos</option>
        <option value="Curso 5">Marketing</option></select
      ><br />
      Comentarios:<br />
      <textarea v-model="comentarios" class="border border-black"></textarea>
    </div>

    <div class="m-5 font-medium">
      Paterno: {{ paterno }}<br />
      Materno: {{ materno }}<br />
      Nombres: {{ nombres }}<br />
      Sexo: {{ sexo }}<br />
      Materia: {{ materia }}<br />
      Comentarios: {{ comentarios }}
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const paterno = ref("");
const materno = ref("");
const nombres = ref("");
const sexo = ref("");
const materia = ref("");
const comentarios = ref("");
</script>
