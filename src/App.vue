<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">MATERIAL DESIGN</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <LPSecurities />
      <SecurityGarantee />
      <OtherSecurityes />
      <TyingSecurityes />
      <Message />
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import LPSecurities from './components/LPSecurities'
import SecurityGarantee from './components/SecurityGarantee'
import OtherSecurityes from './components/OtherSecurityes'
import TyingSecurityes from './components/TyingSecurityes'
import Message from './components/Message'

export default {
  name: 'App',
  components: {
    HelloWorld,
    LPSecurities,
    SecurityGarantee,
    OtherSecurityes,
    TyingSecurityes,
    Message
  },
  data () {
    return {
      //
    }
  }
}
</script>
