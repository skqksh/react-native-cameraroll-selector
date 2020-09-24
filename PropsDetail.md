## Props Detail (\* : required)

| Props             | type                                          | default                              | etc                                                          |
| ----------------- | --------------------------------------------- | ------------------------------------ | ------------------------------------------------------------ |
| \*callback        | func                                          |                                      | (selectedImages:PhotoProps[],currentImage:PhotoProps)=>void  |
| assetType         | CameraRoll.GroupType                          | "Photos"                             | "ALL","Videos","Photos"                                      |
| maximum           | number                                        | 15                                   | To use this option,`selectSingleItem` option must be `false` |
| selectSingleItem  | boolean                                       | false                                | If `true` ,`maximum` option is ignored                       |
| selectedImagesUri | string[]                                      | []                                   | Set uri array with which is returned by callback             |
| selectedMarker    | JSX.Element \| (selected:number)=>JSX.Element | 'circle mark'                        | 'selected' is starts from 1                                  |
| loadingOption     | {                                             |                                      |                                                              |
|                   | initialLoader?: JSX.Element                   | `<ActivityIndicator size="large" />` | initialLoader: It's located at bottom of the photos          |
|                   | }                                             |                                      |                                                              |
| zoomImageOption   | {                                             |                                      |                                                              |
|                   | closeButton?: JSX.Element                     | close image                          |                                                              |
|                   | closeContainerStyle?: ViewStyle               |                                      |                                                              |
|                   | }                                             |                                      |                                                              |
| imageListOption   | {                                             |                                      |                                                              |
|                   | initialNumToRender?: number                   | 5                                    | Flatlist's props                                             |
|                   | containerWidth?: number                       | window.width                         | You can use react-native Dimensions to get window width      |
|                   | ListEmptyComponent?: JSX.Element              |                                      |                                                              |
|                   | imagesPerRow?: number                         | 3                                    | Not Recommend to be over 10                                  |
|                   | imageMargin?: number                          | 5                                    |                                                              |
|                   | }                                             |                                      |                                                              |
| cameraOption      | {                                             |                                      |                                                              |
|                   | cameraButtonIcon?: JSX.Element                | Camera png image                     |                                                              |
|                   | cameraPreviewProps?: RNCameraProps            | RNCameraProps                        | Props of the `react-native-camera`                           |
|                   | cameraPreviewStyle?: ViewStyle                |                                      |                                                              |
|                   | cameraFlipIcon?: JSX.Element                  | Flip png image                       |                                                              |
|                   | cameraCaptureIcon?: JSX.Element               | Circle mark                          |                                                              |
|                   | }                                             |                                      |                                                              |
| headerOption      | {                                             |                                      |                                                              |
|                   | headerContainerStyle?: ViewStyle             |                                      |                                                              |
|                   | headerLeftStyle?: ViewStyle                  |                                      |                                                              |
|                   | headerLeftComponent?: JSX.Element            |                                      |                                                              |
|                   | headerCenterStyle?: ViewStyle                |                                      |                                                              |
|                   | headerCenterComponent?: JSX.Element          | Menu text button                     | Text button for get album, you can choose a specific folder  |
|                   | headerRightStyle?: ViewStyle                 |                                      |                                                              |
|                   | headerRightComponent?: JSX.Element           | Photo image                          | Button to take photo                                         |
|                   | }                                             |                                      |                                                              |
