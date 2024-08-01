<template>
    <v-container>
      <v-row>
        <v-col cols="12">
          <v-btn class="hover-button" outlined>
            Hover over me
          </v-btn>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <style>
  .hover-button {
    transition: background-color 0.3s ease;
  }
  
  .hover-button:hover {
    background-color: #4caf50; /* Màu xanh lá cây */
    color: white; /* Màu chữ */
  }
  </style>
  