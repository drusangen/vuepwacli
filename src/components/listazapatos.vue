<template>
    <v-container fluid grid-list-md>
        <v-layout row wrap>
            <v-flex v-for="cliente in 20" :key="cliente.id" d-flex xs12 sm6 md4 xl3>
                <v-card color="primary" class="white--text elevation-3">
                    <v-container  grid-list-lg>
                        <v-layout row>
                                <div>
                                    <div class="headline">Drusangen</div>
                                    <div>Ariana</div>
                                </div>
                                <v-spacer></v-spacer>
                                <v-btn fab small color="accent">
                                    <v-icon>edit</v-icon>
                                </v-btn>
                        </v-layout>
                    </v-container>
                </v-card>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
  data () {
    return {
      clientes: [
        {
          nombre: 'Boris',
          deuda: 150
        }
      ]
    }
  },
  computed: {
  }
}
</script>
