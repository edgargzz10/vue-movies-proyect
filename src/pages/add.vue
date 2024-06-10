<template>   
  
    <v-container>
      <v-row>        
        <v-sheet class="mx-auto pa-6 ma-6" width="800">
            <h2 class="text-h4 mb-4">Insert New Movie</h2>
            <v-form fast-fail>
                <v-text-field
                    label="Titulo"
                    prepend-icon="mdi-format-title"
                ></v-text-field>

                <v-text-field
                    label="Description"
                    prepend-icon="mdi-text-long "

                ></v-text-field>

                <v-text-field
                    label="Year"
                    prepend-icon="mdi-calendar-blank" 
                    ></v-text-field>
                    <v-file-input label="Movie Image"></v-file-input>

                <v-btn class="mt-2" type="submit" block>Submit</v-btn>
            </v-form>
            </v-sheet>        
      </v-row>
    </v-container>
  </template>
  
  <script setup>
    //
  </script>
  