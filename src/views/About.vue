<template>
  <div>
    <v-app>
      <v-toolbar dark>
        <div class="flex-grow-1"></div>

        <v-toolbar-items class="alignRight">
          <v-btn text>Dashboard</v-btn>
          <v-btn text>Accounts</v-btn>
          <v-btn text>Settings</v-btn>
        </v-toolbar-items>
        
      </v-toolbar>

      <v-app>
        <v-carousel>
          <v-carousel-item
            v-for="(color, i) in colors"
            :key="color"
          >
            <v-sheet
              :color="color"
              height="100%"
              tile
            >
              <v-row
                class="fill-height"
                align="center"
                justify="center"
              >
                <div class="display-3">Slide {{ i + 1 }}</div>
              </v-row>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
      </v-app>
      <h1>Employee Information</h1>
      <v-app>
        <v-simple-table fixed-header height="300px">
        <thead>
          <tr>
            <th class="text-left">Name</th>
            <th class="text-left">Rate Per Hour</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in desserts" :key="item.name">
            <td>{{ item.name }}</td>
            <td>{{ item.calories }}</td>
          </tr>
        </tbody>
      </v-simple-table>
      </v-app>
    </v-app>
    
  </div>
  
</template>

<script>
export default {
  data: () => ({
      elevateOnScroll: false,
      hideOnScroll: false,
      fadeOnScroll: false,
      fadeImgOnScroll: false,
      invertedScroll: false,
      collapse: false,
      collapseOnScroll: false,
      shrinkOnScroll: false,
      extended: false,
      color: 'accent',
      colors: ['primary', 'accent', 'warning lighten-2', 'teal', 'orange'],
      desserts: [
          {
            name: 'John Doe',
            calories: 159,
          },
          {
            name: 'John Does',
            calories: 237,
          },
          {
            name: 'John Doeaa',
            calories: 262,
          },
          {
            name: 'John Doess',
            calories: 305,
          },
          {
            name: 'John Doed',
            calories: 356,
          },
        ],
    }),
    
}
</script>