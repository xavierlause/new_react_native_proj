https://medium.com/react-native-training/learning-to-test-react-native-with-jest-part-1-f782c4e30101

- check dependency:
npm ls jest-environment-node

- install jest-cli with the same version of jest:
npm install jest-cli --save
OR
npm i jest-cli@22.4.3 --save-dev

- test it:
npm test

- if failed, check .babelrc format!!!

- If run test coverage the node_module, try:
  "jest": {
    "preset": "react-native",
    "transformIgnorePatterns": [
      "node_modules/(?!.*)"
    ]
  }
