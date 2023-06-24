```lang-xml
    <load id="meshes">
        <model id="shapes" src="../path/to/collection.obj"/>
    </load>
    <root id="myScene">
        <model id="model_id_001" mesh="shapes" subset="Shape_S" diffuse="crate" tex0mult="1" pos="0,1,0" scale="1"/>
    </root>
```

## Model

### Properties

* `id` required
* `mesh` required 
    * native_plane
    * native_sphere
    * native_cube
