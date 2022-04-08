![AssetStreaming Banner](./Media/banner.png "AssetStreaming")

# AssetStreaming

AssetStreaming was built to demonstrate how to handle world loading without loading everything into memory at once. For more details and explanations you can visit our [Guide to Asset Streaming in Open World Game](https://developer.oculus.com/blog/now-available-guide-to-asset-streaming-in-open-world-games-/). More documentation that explains the ideas and the approach behind this project can be found [here](https://developer.oculus.com/documentation/unity/po-assetstreaming/).

This codebase is availabale as a reference to help you setup your own asset streaming project. Unity-AssetStreaming is under the license found [here](LICENSE) unless otherwise specified.

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.

## Licenses
The *[Demo Assets](./Assets/DemoAssets/)* used in this project are released under the *[Oculus Examples License](./Assets/DemoAssets/LICENSE.txt)*.

The *Oculus Integration* package is released under the *[Oculus SDK License Agreement](./Assets/Oculus/LICENSE.txt)*.

## Getting started

First, ensure you have Git LFS installed by running this command:
```sh
git lfs install
```

Then, clone this repo using the "Code" button above, or this command:
```sh
git clone https://github.com/oculus-samples/Unity-AssetStreaming.git
```

To run the sample, open the project folder in *Unity 2019.4.34f1* or newer. Load the [Assets/Scenes/Startup](Assets/Scenes/Startup.unity) scene.
## Oculus Integration Package
In order to keep the project simple, we kept only the required features from [Oculus Integration](https://assetstore.unity.com/packages/tools/integration/oculus-integration-82022). We kept [VR](Assets/Oculus/VR) and [Platform](Assets/Oculus/Platform). To update it, import the updated Asset Store package, and select only VR and Platform.

## Third-Party Libraries
In our implementation of the LOD Generator, we used a package from the Asset Store called [Mesh Baker](https://assetstore.unity.com/packages/tools/modeling/mesh-baker-5017). We highly recommend using Mesh Baker to create texture atlases and combine your meshes. Alternatively, you could write your own or get a license for something like Simplygon.

For Licenses reasons we didn't include [Mesh Baker](https://assetstore.unity.com/packages/tools/modeling/mesh-baker-5017) in the project.

# Conversion to use Addressables
We detailed how we converted the original Asset Streaming project to use Unity Addressables system [here](./ConversionToAddressables.md).
