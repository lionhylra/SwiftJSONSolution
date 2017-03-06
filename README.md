# SwiftJSONSolution
Provide an efficient solution to convert objects between Swift objects(struct) and JSON.
<br/><br/><br/>
## Table of contents
### [1. JSON to Swift](#JSON2Swift)
### [2. Swift to JSON](#Swift2JSON)
<br/><br/><br/>
### <a name="JSON2Swift"></a>1. JSON to Swift Solution

###### TODO:

- [x] load local JSON file
- [x] display JSON loaded from URL using "pretty" format
- [x] add a feature: "add properties that doesn't exist in JSON file"
- [ ] deal with situation where a arry contains different objects
- [ ] enhance the function "loading JSON via url"
- [ ] flash JSON objects when editting
- [x] add code highlight (low priority for now)


Since Swift doesn't support dynamicly mapping JSON to struct (as explained in this <a href="https://developer.apple.com/swift/blog/?id=37" target="_blank">Swift blog</a>), the fastest way to generate model from JSON seems to be generating the code and initialisers with JSON properties.

The app **JSON2Swift** is a straightforward and easy to use tool to generate swift models. It also supports full customization of a model and properties when it is required.

Here is the tutoral for JSON2Swift:

0. Download the app from [macOS App Store](https://itunes.apple.com/us/app/json2swift/id1208964041?ls=1&mt=12)
1. Copy & Paste JSON content to the input text field, or enter the URL for JSON and load it. (Note: the app currently only support JSON whose root is a dictionay structure.)
  ![Screenshot](/tutorial1.png)
2. Enter the meaningful name of the model to replace the generated model name.
  ![Screenshot](/tutorial22.png)
3. Click the export button. Optionally you can enter the information of your project to generate the header of swift file.
  ![Screenshot](/tutorial3.png)

#### If there is any problem regarding using the software, please raise an issue here.

### <a name="Swift2JSON"></a>2. Swift to JSON Solution

Luckily, by implementing reflection using Mirror, it is feasible to implement this feature in the code. Please see the details in another repository [YHJSONGenerator](https://github.com/lionhylra/YHJSONGenerator)
