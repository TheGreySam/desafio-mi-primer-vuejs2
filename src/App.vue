<template>

<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">RUN</th>
      <th scope="col">Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(persona, $index) in personas" :key="$index">
      <td>{{ $index}}</td>
      <td>{{ persona.nombre}}</td>
      <td>{{ persona.apellido}}</td>
      <td>{{ persona.rut}}</td>
      <td>{{ persona.fechaDeNacimiento}}</td>
      <td>{{ persona.edad}}</td>
      
      
    </tr>
    <tr>
      
    </tr>
  </tbody>
</table>
</template>

<script>

export default {
  name: "App",
    data: () => ({
      personas: [
        {
          nombre: "Jose",
          apellido: "Pérez",
          rut: "123456-2",
          edad: 52,
          fechaDeNacimiento: "12-04-67", 
         },
         {
          nombre: "María",
          apellido: "Rodríguez",
          rut: "654321-1",
          edad: 29,
          fechaDeNacimiento: "30-11-90", 
         },
         {
          nombre: "Manuel",
          apellido: "Patiño",
          rut: "14223456-6",
          edad: 60,
          fechaDeNacimiento: "02-12-59", 
         },
      ],
  })
};
</script>

<style>

</style>