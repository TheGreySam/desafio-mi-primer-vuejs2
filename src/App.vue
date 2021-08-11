<template>

<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">RUT</th>
      <th scope="col">Edad</th>
      <th scope="col">Fecha de Nacimiento</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(persona, $index) in personas" :key="$index">
      <td>{{ $index}}</td>
      <td>{{ persona.nombre}}</td>
      <td>{{ persona.apellido}}</td>
      <td>{{ persona.rut}}</td>
      <td>{{ persona.edad}}</td>
      <td>{{ persona.fechaDeNacimiento}}</td>
      
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
          nombre: "Angela",
          apellido: "Vidal",
          rut: "1.234.567-7",
          edad: 20,
          fechaDeNacimiento: "01-01-2000", 
         },
         {
          nombre: "Gonzalo",
          apellido: "Jara",
          rut: "1.234.567-7",
          edad: 20,
          fechaDeNacimiento: "01-01-2000", 
         },
         {
          nombre: "Seba",
          apellido: "Gómez",
          rut: "1.234.567-7",
          edad: 20,
          fechaDeNacimiento: "01-01-2000", 
         },
      ],
  })
};
</script>

<style>

</style>