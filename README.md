# node-critools

Node.js library for extracting Cri-based audio files originally written by [kohos](https://github.com/kohos/CriTools). 
This library is created as an interface for other node.js apps to be able to access the functionalities of the tool.

## Usage
```
$ npm install critools
```

### Example

```
import {acb2wavs} from "critools";
await acb2wavs("./test.acb", key, "./");
```

### API

```
acb2hcas(acbPath, key?, hcaDir?, type?, skip?)
acb2wavs(acbPath, key?, wavDir?, volume?, mode?, skip?)
decryptAcb(acbPath, key?, type?)
awb2hcas(awbPath, key?, hcaDir?, type?, skip?)
awb2wavs(awbPath, key?, wavDir?, volume?, mode?, skip?)
decryptAwb(awbPath, key?, type?)
decodeHca(buffer, key?, awbKey?, volume?)
decodeHcaToWav(buffer, key?, awbKey?, wavPath?, volume?, mode?)
decryptHca(buffer, key?, awbKey?, type?, hcaPath?)
extractCpk(cpkPath, output?)
parseUtf(buffer, toString?)
viewUtf(acbPath, outputPath?)
```

## License

Released under the [MIT License](https://github.com/djzmo/node-critools/LICENSE).

## Credits
* [kohos/CriTools](https://github.com/kohos/CriTools)
