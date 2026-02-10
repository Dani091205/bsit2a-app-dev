<template>
  <div>
    <v-row>
      <v-col cols="12" md="3">
        <v-card height="120" elevation="0" color="grey">
          <v-card-text>
            <v-row align="center">
              <v-col>
                <v-icon size="80">mdi-account</v-icon>
              </v-col>
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h6">Student</v-col>
                  <v-col cols="12" class="text-right text-h3 font-weight-bold"
                    >10</v-col
                  >
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" elevation="0" color="grey">
          <v-card-text>
            <v-row align="center">
              <v-col>
                <v-icon size="80">mdi-account</v-icon>
              </v-col>
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h6">Account</v-col>
                  <v-col cols="12" class="text-right text-h3 font-weight-bold"
                    >234</v-col
                  >
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" elevation="0" color="grey">
          <v-card-text>
            <v-row align="center">
              <v-col>
                <v-icon size="80">mdi-account</v-icon>
              </v-col>
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h6">Expenses</v-col>
                  <v-col cols="12" class="text-right text-h3 font-weight-bold"
                    >62</v-col
                  >
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="12" md="3">
        <v-card height="120" elevation="0" color="grey">
          <v-card-text>
            <v-row align="center">
              <v-col>
                <v-icon size="80">mdi-account</v-icon>
              </v-col>
              <v-col>
                <v-row no-gutters>
                  <v-col cols="12" class="text-right text-h6"
                    >New employees</v-col
                  >
                  <v-col cols="12" class="text-right text-h3 font-weight-bold"
                    >34</v-col
                  >
                </v-row>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>

      <v-col cols="4" md="8">
        <v-card height="300" elevation="0" color="grey"> 
          <v-data-table
    :headers="headers"
    :items="plants"
    density="compact"
    item-key="name"
  ></v-data-table>
        </v-card>
      </v-col>

      <v-col cols="3" md="4">
        <v-row>
          <v-col>
            <v-card height="100" color="grey"> </v-card>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <v-card height="100" color="grey"> </v-card>
          </v-col>
        </v-row>
        <v-row>
          <v-col> <v-card height="100" color="grey"> </v-card></v-col>
        </v-row>
      </v-col>
    </v-row>
  </div>
</template>
      
    
      <script setup>
      
  const headers = [
    { title: 'Plant', align: 'start', sortable: false, key: 'name' },
    { title: 'Light', align: 'end', key: 'light' },
    { title: 'Height', align: 'end', key: 'height' },
    { title: 'Pet Friendly', align: 'end', key: 'petFriendly' },
    { title: 'Price ($)', align: 'end', key: 'price' },
  ]

  const plants = [
    {
      name: 'Fern',
      light: 'Low',
      height: '20cm',
      petFriendly: 'Yes',
      price: 20,
    },
    {
      name: 'Snake Plant',
      light: 'Low',
      height: '50cm',
      petFriendly: 'No',
      price: 35,
    },
    {
      name: 'Monstera',
      light: 'Medium',
      height: '60cm',
      petFriendly: 'No',
      price: 50,
    },
    {
      name: 'Pothos',
      light: 'Low to medium',
      height: '40cm',
      petFriendly: 'Yes',
      price: 25,
    },
    {
      name: 'ZZ Plant',
      light: 'Low to medium',
      height: '90cm',
      petFriendly: 'Yes',
      price: 30,
    },
    {
      name: 'Spider Plant',
      light: 'Bright, indirect',
      height: '30cm',
      petFriendly: 'Yes',
      price: 15,
    },
    {
      name: 'Air Plant',
      light: 'Bright, indirect',
      height: '15cm',
      petFriendly: 'Yes',
      price: 10,
    },
    {
      name: 'Peperomia',
      light: 'Bright, indirect',
      height: '25cm',
      petFriendly: 'Yes',
      price: 20,
    },
    {
      name: 'Aloe Vera',
      light: 'Bright, direct',
      height: '30cm',
      petFriendly: 'Yes',
      price: 15,
    },
    {
      name: 'Jade Plant',
      light: 'Bright, direct',
      height: '40cm',
      petFriendly: 'Yes',
      price: 25,
    },
  ]
</script>
<style></style>