# MobileVLCKit-SPM Lite Version

without dsyms and simulator support 

MobileVLCKit Swift Package Manager Support

in package.swift
```
dependencies: [
  .package(url: "https://github.com/MobileVLCKit-SPM/MobileVLCKit-SPM-Lite", from: "3.5.1"),
]
...
targets: [
          .target(
              ...
              dependencies: [
                .product(name: "MobileVLCKit", package: "MobileVLCKit-SPM-Lite",condition: TargetDependencyCondition.when(platforms: [.iOS])),
              ],
             ...
           )
        ]
)
```


xcode project ：

download mobilevlc framework from : https://download.videolan.org/pub/cocoapods/prod
