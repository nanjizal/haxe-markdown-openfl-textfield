# Markdown for OpenFL

Extends the Haxe [Markdown](https://lib.haxe.org/p/markdown) library to add support for the OpenFL `TextField` class.

## Install

Run the following command in a terminal.

```sh
haxelib install markdown-openfl-textfield
```

Then, add the following line to your OpenFL [_project.xml_](https://lime.software/docs/project-files/xml-format/) file.

```xml
<haxelib name="markdown-openfl-textfield" />
```

## Usage

The following example displays Markdown in an `openfl.text.TextField` using its `htmlText` property.

```hx
var rawMarkdown = "Hello, **world**!";
var htmlText = TextFieldMarkdown.markdownToHtml(rawText);

var textField = new TextField();
textField.htmlText = htmlText;
this.addChild(htmlText);
```
