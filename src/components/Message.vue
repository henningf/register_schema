<template>
    <v-layout row>
        <v-flex xs12>
      <v-card>
        <v-toolbar color="cyan" dark>

          <v-toolbar-title>Beskjed til depot</v-toolbar-title>

          <v-spacer></v-spacer>

          <v-btn icon>
            <v-icon>note_add</v-icon>
          </v-btn>
        </v-toolbar>
            <v-layout row wrap>
            <v-flex xs10>
            <blockquote class="blockquote">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum maiores modi quidem veniam, expedita quis laboriosam, ullam facere adipisci, iusto, voluptate sapiente corrupti asperiores rem nemo numquam fuga ab at.</blockquote>
            </v-flex>
            <v-flex xs2 text-xs-right>
                <v-btn icon>
            <v-icon>edit</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>delete</v-icon>
          </v-btn>
            </v-flex>
            </v-layout>
      </v-card>
    </v-flex>
    </v-layout>
</template>

<script>
export default {
    data () {
      return {
      }
    }
}
</script>

<style>

</style>


  
