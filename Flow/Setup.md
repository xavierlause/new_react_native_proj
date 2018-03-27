# Install Flow globally:

```
sudo npm i flow-bin -g
```


* After react-native 0.46:
https://medium.com/react-native-training/getting-started-with-react-native-and-flow-d40f55746809


* cehck .flowconfig, see the version of flow:
[version]
^0.68.0

* then run
npm i flow-bin@0.68.0 --save-dev


* then run the following code and fix the error if exist:
npm run flow

* if react-native code / node_module are checked: do the following step:
1) ignore in .flowconfig => .*/node_modules/.*
2) create flow-typed folder
3) create react-native.js in the folder with codes: 
	declare module 'react-native' {
		declare module.exports: any;
	}
4) add dependency under [lib] in .flowconfig => flow-typed/	

5) Will check the file with the following header:
/**
 * Sample React Native App
 * https://github.com/facebook/react-native
 * @flow
 */
 
* Check .babelrc
 "presets": [["react-native"], ["flow"]]


Flow Documents: https://flow.org/en/docs
