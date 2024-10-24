# 3d-web-viz
3D web visualization experiments (USD, GLTF, 3D tiles, Three.js, etc.)

## USD

USD (Universal Scene Description) is a framework developed by Pixar for defining, composing, simulating, and collaborating on 3D data. It enables complex scene descriptions, consisting of geometry, shading, animation, lighting, and other elements, to be efficiently stored and shared across multiple teams and software. USD is highly scalable and suitable for workflows in VFX, animation, gaming, and other industries dealing with complex 3D scenes.

A USD file is a plain text file (or binary) with a .usd, .usda (ASCII), or .usdc (binary compressed) extension. Here's a simple example in the USD ASCII format (.usda):

```usda
(
    doc = "A simple USD scene"
)

def Sphere "mySphere" {
    float3 xformOp:translate = (0, 0, 0)
    uniform token[] xformOpOrder = ["xformOp:translate"]
    double radius = 1
}
```
[sphere.usda](./usd/sphere.usda)

This defines a scene containing a single sphere named mySphere positioned at the origin (0, 0, 0) with a radius of 1.
