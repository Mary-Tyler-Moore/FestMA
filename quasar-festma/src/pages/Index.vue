<template>
  <q-page class="container scene">

    <a-scene arjs='debugUIEnabled: false;'>

      <a-marker
        id='frac1'
        type='pattern'
        url='statics/marker/pt-frac1.patt'
      >
        <a-plane
          color="white"
          width="5"
          position="4.5 1 0"
          rotation="-90 0 0"
        ></a-plane>
        <a-text
          value="Obra: “Disponibilita” (1981)
            Antonio Peticov"
          align="center"
          color="black"
          width="5"
          position="5 1.1 0"
          rotation="-90 0 0"
        ></a-text>

        <a-plane
          src="statics/disponibilita.jpg"
          width="3.8"
          height="5.1"
          rotation="-90 0 0"
        >
        </a-plane>
      </a-marker>

      <a-box
        color="yellow"
        gps-entity-place="latitude: 32.428387; longitude: 81.76802839999999"
        position="0 30 0"
      />

      <a-camera
        gps-camera
        rotation-reader
      ></a-camera>
    </a-scene>
  </q-page>
</template>

<style>
.scene {
  z-index: 100 !important;
}
</style>

<script>

export default {
  name: 'PageIndex'
}
</script>
