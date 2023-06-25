<template>
  <div ref="canvas"></div>
</template>

<script setup>
import * as THREE from "three";

const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(
  75,
  window.innerWidth,
  window.innerHeight
);

const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(window.innerWidth, window.innerHeight);
this.$refs.canvas.appendChild(renderer.domElement);

const geomitry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.MeshStandardMaterial({
  color: 0x00ff00,
});
const cube = new THREE.Mesh(geomitry, material);
scene.add(cube);

camera.position.z = 5;
</script>
