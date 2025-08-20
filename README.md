# X3D-PBR-Studio
An open-source, browser-based PBR authoring, baking, and rendering tool for the X3D v4 standard

### PBR Mapping Details (Three.js → X3D v4)
- baseColorFactor ← material.color + material.opacity
- metallicFactor ← material.metalness
- roughnessFactor ← material.roughness
- emissiveFactor ← material.emissive
- clearcoatFactor / clearcoatRoughnessFactor ← MeshPhysicalMaterial fields
- ior, sheen, sheenColorFactor ← MeshPhysicalMaterial fields if present
- baseTexture ← material.map
- metallicRoughnessTexture ← material.metalnessRoughnessMap (or fallback to metalnessMap / roughnessMap)
- normalTexture ← material.normalMap
- occlusionTexture ← material.aoMap
- emissiveTexture ← material.emissiveMap
