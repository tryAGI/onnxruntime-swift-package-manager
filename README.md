> **Independent archival mirror — not maintained or endorsed by Microsoft.**
>
> This repository preserves ONNX Runtime SwiftPM version **1.24.2** while the
> upstream Microsoft repository is unavailable. The original, previously
> published Git commit `b7fb7f7dea8a2469e6335d95a61b8f36d0dc83b2` is
> preserved unchanged in this repository's ancestry. The only changes to the
> Swift package manifest replace the two unavailable binary download URLs
> with the independently hosted **exact same ZIP files**, not rebuilt binaries:
>
> - `pod-archive-onnxruntime-c-1.24.2.zip` SHA-256:
>   `f7100a992d2a8135168c8afd831e6a58b465349101982aa58b3e11d36e600b54`
> - `pod-archive-onnxruntime-extensions-c-0.13.0.zip` SHA-256:
>   `346522d1171d4c99cb0908fa8e4e9330a4a6aad39cd83ce36eb654437b33e6b5`
>
> Source provenance: Microsoft commit retained in the existing Advantage lock,
> verified against several public forks. The original ZIPs were recovered from
> a pre-existing pinned SwiftPM cache and each archive was byte-checked against
> Microsoft's previously published package manifest and again against GitHub's
> uploaded-release digest. See [archival release assets](https://github.com/tryAGI/onnxruntime-swift-package-manager/releases/tag/assets-1.24.2).
>
> No independent security certification is implied. Review any future official
> Microsoft advisory before upgrading or retiring this mirror.

**For reproducible SwiftPM builds** (compatible public products and imports):

```swift
.package(url: "https://github.com/tryAGI/onnxruntime-swift-package-manager", exact: "1.24.2")
```

---

# Swift Package Manager for ONNX Runtime

A light-weight repository for providing [Swift Package Manager (SPM)](https://www.swift.org/package-manager/) support for [ONNXRuntime](https://github.com/microsoft/onnxruntime). The ONNX Runtime native package is included as a binary dependency of the SPM package.


SPM is the alternative to CocoaPods when desired platform to consume is mobile iOS.

## Note

The `objectivec/` directory is copied from the [ORT repo](https://github.com/microsoft/onnxruntime/tree/main/objectivec) and it's expected to match. It will be updated periodically/before release to merge new changes.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
