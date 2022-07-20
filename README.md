# React Native QR Code Scanner

A highly customizable QR Code scanner based on  **[react-native-qrcode-scanner-view](https://github.com/MarnoDev/react-native-qrcode-scanner-view)**.

---

## Features

- Pure JS code
- Support Android and iOS
- Support React Native 0.60+
- Support scan QR code, Bar code
- Scanning interface can be customized

## Props

|Prop|Type|Default|Optional|
| :-------------------: | :----: | :----------------------------------------------------------------------------------------------: | :---: |
|       maskColor       | string |                                            #0000004D                                             | true  |
|       rectStyle       | object | height: 300, <br>width: 300, <br>borderWidth: 0, <br>borderColor: '#000000', <br>marginBottom: 0 | true  |
|      cornerStyle      | object |            height: 32, <br>width: 32, <br>borderWidth: 6, <br>borderColor: '#E65100'             | true  |
|   cornerOffsetSize    | number |                                                0                                                 | true  |
|     isShowCorner      |  bool  |                                               true                                               | true  |
|     scanBarStyle      | object |             marginHorizontal: 8, <br>borderRadius: 2, <br>backgroundColor: '#E65100'             | true  |
|     isShowScanBar     |  bool  |                                               true                                               | true  |
|  scanBarAnimateTime   | number |                                               3000                                               | true  |
| scanBarAnimateReverse |  bool  |                                              false                                               | true  |
|     scanBarImage      |  any   |                                                                                                  | true  |
|       hintText        | string |                                                                                                  | true  |
|     hintTextStyle     | object |      color: '#fff', <br>fontSize: 14, <br>backgroundColor: 'transparent', <br>marginTop: 32      | true  |
|   renderHeaderView    |  func  |                                                -                                                 | true  |
|   renderFooterView    |  func  |                                                -                                                 | true  |
|     onScanResult      |  func  |                                                -                                                 | false |
|     scanInterval      | number |                                               2000                                               | true  |
|        torchOn        |  bool  |                                              false                                               | true  |
|       userFront       |  bool  |                                              false                                               | true  |
