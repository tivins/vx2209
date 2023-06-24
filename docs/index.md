## Scene definition (XML)

```xml
<scene>
    <load id="meshes">
        <model id="shapes" src="../path/to/collection.obj"/>
    </load>
    <root id="myScene">
        <model id="model_id_001" mesh="shapes" subset="Shape_S" diffuse="crate" tex0mult="1" pos="0,1,0" scale="1"/>
    </root>
</scene>
```

## Info

### Vector notation

A single or three float values. (ex: `attr=".75"` equals `attr=".75,.75,.75"`).

## `<model>` node

Example:
```xml
<model 
    id="model_id_001" 
    mesh="shapes" 
    subset="Shape_S" 
    diffuse="crate"
    tex0mult="1" 
    pos="0,1,0" 
    scale=".75"
    />
```

* `id` required
* `mesh` required
  May contains :
    * `native_plane`
    * `native_sphere`
    * `native_cube`
    * or a Mesh ID.
* `subset` (optional). Only if `mesh` is a custom mesh. If defined, the group name.
* `diffuse` Identifier of the texture.
* `pos` Position as ([vector](#vector-notation)).
* `scale` Model scale factor as ([vector](#vector-notation)).
