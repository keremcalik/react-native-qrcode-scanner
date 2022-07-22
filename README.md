# React Native QR Code Scanner

A highly customizable QR Code scanner based on  **[react-native-qrcode-scanner-view](https://github.com/MarnoDev/react-native-qrcode-scanner-view)**.

# What I Changed ?

**[I had this issue](https://github.com/MarnoDev/react-native-qrcode-scanner-view/issues/72)** and I didn't get any solution on this page.
There is problem with scanBarStyle and somebody has recommended remove scanBarStyle property. I changed this property in original QR Scanner file instead of removing.
Also there is problem with componentDidMount() and componentWillUnmount() functions. I fixed this problem.

  <code>listener;
  componentDidMount() {
    listener = AppState.addEventListener("change", this.handleAppStateChange);
  }

  componentWillUnmount() {
    listener.remove();
    this.rnCamera && this.rnCamera.pausePreview();
  }</code>
  
---

## Features

- Pure JS code
- Support Android and iOS
- Support React Native 0.60+
- Support scan QR code, Bar code
- Scanning interface can be customized

## Props

|Prop|Type|Default|
| :-------------------: | :----: | :----------------------------------------------------------------------------------------------: |
|       maskColor       | string |                                            #0000004D                                             | 
|       rectStyle       | object | height: 300, <br>width: 300, <br>borderWidth: 0, <br>borderColor: '#000000', <br>marginBottom: 0 | 
|      cornerStyle      | object |            height: 32, <br>width: 32, <br>borderWidth: 6, <br>borderColor: '#E65100'             | 
|   cornerOffsetSize    | number |                                                0                                                 | 
|     isShowCorner      |  bool  |                                               true                                               | 
|     scanBarStyle      | object |             marginHorizontal: 8, <br>borderRadius: 2, <br>backgroundColor: '#E65100'             | 
|     isShowScanBar     |  bool  |                                               true                                               | 
|  scanBarAnimateTime   | number |                                               3000                                               | 
| scanBarAnimateReverse |  bool  |                                              false                                               | 
|     scanBarImage      |  any   |                                                                                                  | 
|       hintText        | string |                                                                                                  | 
|     hintTextStyle     | object |      color: '#fff', <br>fontSize: 14, <br>backgroundColor: 'transparent', <br>marginTop: 32      | 
|   renderHeaderView    |  func  |                                                -                                                 | 
|   renderFooterView    |  func  |                                                -                                                 | 
|     onScanResult      |  func  |                                                -                                                 | 
|     scanInterval      | number |                                               2000                                               | 
|        torchOn        |  bool  |                                              false                                               | 
|       userFront       |  bool  |                                              false                                               | 
