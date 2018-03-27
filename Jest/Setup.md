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
  
- Make a simple test in ./__tests__/App.js:
  test("adds 1 + 2 to equal 3", () => {
    expect((1+2)).toBe(3);
  });
  
  
==============================
Tools : Enzyme (Airbnb)

http://airbnb.io/projects/enzyme/

- Installation:
npm i --save-dev enzyme

Check if Exist:
npm i --save-dev react-addons-test-utils
npm i --save-dev react-dom
