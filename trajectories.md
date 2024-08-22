---
layout: page
title: Trajectories
---

The four outdoor trajectories can be visualized on the interactive map below. We use the same colors presented in the paper. Click on a trajectory to see its name.

<div style="text-align: center;">
  <iframe src="https://www.google.com/maps/d/u/0/embed?mid=15RbG2iCkygBUAvPHpycijGC5UoVxvPE&ehbc=2E312F&noprof=1" width="100%" height="480"></iframe>
</div>

Our dataset includes an indoor map built with advanced stationary LiDAR scanners. The 3D point cloud of the garage can be used for various indoor navigation research purposes.

<div>
  <script src="https://cdn.jsdelivr.net/npm/three@0.155.0/build/three.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/three@0.155.0/examples/js/loaders/PCDLoader.js"></script>
  <script>
    // Set up the scene, camera, and renderer
    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    const renderer = new THREE.WebGLRenderer();
    renderer.setSize(window.innerWidth, window.innerHeight);
    document.body.appendChild(renderer.domElement);

    // Add light to the scene
    const light = new THREE.AmbientLight(0x404040); // soft white light
    scene.add(light);

    // Load the PCD file
    const loader = new THREE.PCDLoader();
    loader.load('/assets/map/Indoor_garage_3D_map_LLF.pcd', function (points) {
        scene.add(points);
        camera.position.z = 2;  // Adjust camera position if needed
        animate();
    });

    // Render loop
    function animate() {
        requestAnimationFrame(animate);
        renderer.render(scene, camera);
    }

    // Handle window resize
    window.addEventListener('resize', function () {
        const width = window.innerWidth;
        const height = window.innerHeight;
        renderer.setSize(width, height);
        camera.aspect = width / height;
        camera.updateProjectionMatrix();
    });
  </script>

</div>
