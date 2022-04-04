<template>
  <v-container>
    <v-row justify="center" align="center">
      <v-col cols="12">
        <h1 class="text-center">Digital visas provided by European countries</h1>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-data-table
          :headers="europeanCountries"
          :items="europeanVisas"
        ></v-data-table>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import {europeanCountries} from '~/models/europeanCountries';
import {europeanVisas} from '~/models/europeanVisas';
</script>