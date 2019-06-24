<template>
    <v-layout row>
        <v-flex xs12>
      <v-card>
        <v-toolbar color="cyan" dark>

          <v-toolbar-title>Sikkerheter</v-toolbar-title>

          <v-spacer></v-spacer>

          <v-btn icon>
            <v-icon>note_add</v-icon>
          </v-btn>
        </v-toolbar>

        <v-list two-line>
          <template v-for="(item, index) in items">
            <v-subheader
              v-if="item.header"
              :key="item.header"
            >
              {{ item.header }}
            </v-subheader>

            <v-divider
              v-else-if="item.divider"
              :key="index"
              :inset="item.inset"
            ></v-divider>

            <v-list-tile
              v-else
              :key="item.title"
              avatar
              @click="t"
            >
              <v-list-tile-content>
                <v-list-tile-title v-html="item.title"></v-list-tile-title>
                <v-list-tile-sub-title v-html="item.subtitle"></v-list-tile-sub-title>
              </v-list-tile-content>
              <v-btn icon>
            <v-icon>edit</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>delete</v-icon>
          </v-btn>
            </v-list-tile>
          </template>
        </v-list>
      </v-card>
    </v-flex>
    </v-layout>
</template>

<script>
export default {
    data () {
      return {
        items: [
          { header: 'Sikkerheter som er lagt til' },
          {
            title: 'Sikkerhet 1',
            subtitle: "Info rundt sikkerhet 1?"
          },
          { divider: true, inset: true },
          {
            title: 'Sikkerhet 2',
            subtitle: "Info rundt sikkerhet 2?"
          },
          { divider: true, inset: true },
          {
            title: 'Sikkerhet 3',
            subtitle: "Info rundt sikkerhet 3?"
          }
        ]
      }
    }
}
</script>

<style>

</style>
