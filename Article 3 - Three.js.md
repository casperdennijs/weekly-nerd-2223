# Three.js
Three.js is een populaire JavaScript library die wordt gebruikt voor het maken en weergeven van interactieve 3D-computerafbeeldingen in webbrowsers. Het biedt een breed mogelijkheid aan functies en hulpprogramma's die het werken met 3D-afbeeldingen vereenvoudigen, waaronder rendering, animatie, camerabediening, belichtingseffecten en meer.

Three.js maakt gebruik van WebGL, een webstandaard voor het renderen van 3D-afbeeldingen op de GPU, om rendering met hoge prestaties te bereiken in moderne webbrowsers. Het leid veel af van de complexiteit van het werken met WebGL, waardoor het toegankelijker wordt voor ontwikkelaars die geen uitgebreide grafische programmeerervaring hebben.

Voorbeelden van toepassingen die met Three.js zijn gemaakt, zijn onder andere interactieve 3D-visualisaties, games, VR en AR-ervaringen, architecturale visualisaties en het verbeteren van de interactiviteit van websites.

## Voorbeelden
[Sketchfab](https://sketchfab.com/): Een populaire online 3D-modelweergave- en delingsplatform. Het maakt gebruik van Three.js om gebruikers in staat te stellen hun 3D-modellen in realtime te bekijken en te delen in de browser.

[PlayCanvas](https://playcanvas.com/): Een webgebaseerd game-ontwikkelingsplatform dat Three.js als onderliggende technologie gebruikt. Het biedt een volledige 3D-game-engine met ondersteuning voor fysica, animatie en multiplayer-functionaliteit.

[Voxels](https://www.voxels.com/): Een realtime multiplayer-game waarin spelers samenwerken om 3D-constructies te bouwen in een voxelwereld. Het gebruikt Three.js voor het weergeven en bewerken van de voxelomgeving.

## Voorbeeld code
```JS
// Initialiseren van de scene, camera en renderer
var scene = new THREE.Scene();
var camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
var renderer = new THREE.WebGLRenderer();
renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// Geometrie en materiaal voor de kubus
var geometry = new THREE.BoxGeometry();
var material = new THREE.MeshBasicMaterial({ color: 0x00ff00 });
var cube = new THREE.Mesh(geometry, material);
scene.add(cube);

// Camera positie instellen
camera.position.z = 5;

// Render functie
function animate() {
  requestAnimationFrame(animate);

  // Kubus roteren
  cube.rotation.x += 0.01;
  cube.rotation.y += 0.01;
  
  // Renderen van de scene met de camera
  renderer.render(scene, camera);
}

animate();
```
Dit voorbeeld maakt een kubus in een Three.js scene en roteert deze continu. Het resultaat wordt weergegeven op een canvas element in de webpagina. Dit is een basisstructuur waarop je verder kunt bouwen om meer 3D ervaringen te maken met Three.js.

## Conclusie
Three.js is een hele interessante library om je in te gaan verdiepen. Je kan er een heleboele coole werelden bijvoorbeeld mee maken die je naar eigen wensen kan inrichten. Deze kan je vervolgens op het web voor iedereen toegankelijk maken. Maar naast werelden kan je ook hele vette animaties er in maken. Moet wel zeggen dat die allemaal vrij uitdagend en ingewikkeld kan zijn dus je zal wel genoeg tijd en energie erin moeten steken wil je een groot project kunnen maken. Maar wel heel erg de moeite waard om in te verdiepen.

## Bronnen
- https://threejs.org/
- https://threejs.org/docs/
- https://threejs.org/examples/
- https://sketchfab.com/
- https://playcanvas.com/
- https://www.voxels.com/
