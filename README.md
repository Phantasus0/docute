# Demo by Phantasus_

[官方文档](https://docute.egoist.dev/zh/)<Badge type="tip">看这~</Badge>

<ImageZoom 
  src="https://i.loli.net/2018/09/24/5ba8e878850e9.png" 
  :border="true" 
  width="300"
/>

<Note type="warning">

这是一个示例页面

</Note>

```js {highlight:[3,'5-7',12]}
//Test
class SkinnedMesh extends THREE.Mesh {
  constructor(geometry, materials) {
    super(geometry, materials);

    this.idMatrix = SkinnedMesh.defaultMatrix();
    this.bones = [];
    this.boneMatrices = [];
    //...
  }
  update(camera) {
    //...
    super.update();
  }
  static defaultMatrix() {
    return new THREE.Matrix4();
  }
}
```