<script setup lang="ts">
import { LMap, LTileLayer, LControlLayers } from '@vue-leaflet/vue-leaflet'
const zoom = 9;
const drCenter = [18.8050403, -70.6763191]
</script>
<template>
    <LMap v-model="zoom" v-model:zoom="zoom" :center="drCenter">
        <LTileLayer url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"></LTileLayer>
    </LMap>
</template>
