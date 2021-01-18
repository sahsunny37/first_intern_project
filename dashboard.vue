<template>
  <div class="">
     <span style="font-size: 30px; font-weight:bold">Tables</span>
    <span class=" mx-2">included</span>
   
    <v-card>
    <v-card-title>
      <h3>Default Table</h3>
    </v-card-title>
   <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr>
            <th class="text-left">
              <h3>#</h3>
            </th>
            <th class="text-left">
              <h3>First Name</h3>
            </th>
            <th class="text-left">
              <h3>Last Name</h3>
            </th>
            <th class="text-left">
              <h3>Username</h3>
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td rowspan="2">1</td>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>2</td>
            <td>Jaccob</td>
             <td>Thornton</td>
            <td>@TwBoostrap</td>
          </tr>
          <tr>
            <td>3</td>
            <td colspan="2">Larry the Bird</td>
            <td>@twitter</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
    </v-card>

    <v-card>
    <v-card-title>
      <h3>Bootstrap Stripped Table</h3>
    </v-card-title>
   <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr>
            <th class="text-left">
              <h3>#</h3>
            </th>
            <th class="text-left">
              <h3>First Name</h3>
            </th>
            <th class="text-left">
              <h3>Last Name</h3>
            </th>
            <th class="text-left">
              <h3>Username</h3>
            </th>
          </tr>
        </thead>
        <tbody>
          <tr style="background:#ccc">
            <td>1</td>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>2</td>
            <td>Jaccob</td>
             <td>Thornton</td>
            <td>@TwBoostrap</td>
          </tr>
          <tr style="background:#ccc">
            <td>3</td>
            <td>Larry</td> 
            <td>the Bird</td>
            <td>@twitter</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-card-title>
      <h3>Bootstrap Bordered Table</h3>
    </v-card-title>
   <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr>
            <th class="text-left">
              <h3>#</h3>
            </th>
            <th class="text-left">
              <h3>First Name</h3>
            </th>
            <th class="text-left">
              <h3>Last Name</h3>
            </th>
            <th class="text-left">
              <h3>Username</h3>
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td rowspan="2">1</td>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>2</td>
            <td>Jaccob</td>
             <td>Thornton</td>
            <td>@TwBoostrap</td>
          </tr>
          <tr>
            <td>3</td>
            <td colspan="2">Larry the Bird</td>
            <td>@twitter</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
    </v-card>

    <v-card>
    <v-card-title>
      <h3>Tampletes Table</h3>
    </v-card-title>
   <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr class="temp">
            <th class="text-left">
              <h3>#</h3>
            </th>
            <th class="text-left">
              <h3>First Name</h3>
            </th>
            <th class="text-left">
              <h3>Last Name</h3>
            </th>
            <th class="text-left">
              <h3>Username</h3>
            </th>
          </tr>
        </thead>
        <tbody>
         <tr>
            <td rowspan="2">1</td>
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr style="background:#ccc">
            <td>Mark</td>
             <td>Otto</td>
            <td>@mdo</td>
          </tr>
          <tr>
            <td>2</td>
            <td>Jaccob</td>
             <td>Thornton</td>
            <td>@TwBoostrap</td>
          </tr>
          <tr style="background:#ccc">
            <td>3</td>
            <td colspan="2">Larry the Bird</td>
            <td>@twitter</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
    </v-card>
    
  </div>
</template>

<script>

export default {

  }
</script>

<style scoped>
  th{
  border: 1px solid grey;
}
h3{
  color:black;
}
td{
  border: 1px solid grey;
  color:grey;
}
.temp{
  background:teal;
}
.v-card{
  margin-bottom: 50px;
}
span{
  color:grey;
}
</style>