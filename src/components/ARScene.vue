<template>
<div class="hello">
    <!--    <h1>{{ msg }}</h1>-->
    <!--    <div id="myEmbeddedScene" style="  border-style: solid;border-color: red">-->
  <a-scene
      vr-mode-ui="enabled: false;"
      loading-screen="enabled: false;"
      renderer="logarithmicDepthBuffer: true;"
      arjs="trackingMethod: best; sourceType: webcam; debugUIEnabled: false;"
      id="scene"
      embedded
      gesture-detector
  >
    <a-assets>
      <a-asset-item
          id="animated-asset"
          src="../assets/asset.glb"
      ></a-asset-item>
    </a-assets>

    <a-marker
        type="pattern"
        preset="custom"
        url="../assets/marker.patt"
        raycaster="objects: .clickable"
        emitevents="true"
        cursor="fuse: false; rayOrigin: mouse;"
        id="markerA"
    >
      <a-entity
          id="bowser-model"
          scale="11.512728676966768 11.512728676966768 11.512728676966768"
          animation-mixer="loop: repeat"
          gltf-model="#animated-asset"
          class="clickable"
          gesture-handler
      ></a-entity>
    </a-marker>

    <a-entity camera></a-entity>
  </a-scene>
</div>

<!--  </div>-->
</template>

<script>
export default {
    name: 'ARScene',
    props: {
        msg: String,
      // isCameraActive: {
      //     required: true,
      //   default: true
      // }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
#myEmbeddedScene {
    height: 500px;
    width: 500px;
}

h3 {
    margin: 40px 0 0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
