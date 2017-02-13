# &lt;juicy-ace-editor&gt;

> Even <strong>more</strong> embeddable code editor.
> Custom Element - just one tag, and no JS needed to provide
> [Ace](http://ace.c9.io/) - The High Performance Code Editor

## Demo

[Check it live!](http://juicy.github.io/juicy-ace-editor)

[Play & Configure with kitchen sink](http://juicy.github.io/juicy-ace-editor/kitchen-sink.html)

## Features

Besides Ace features, `<juicy-ace-editor>` does:

 - provide extremely clean and easy way to embed it (see [Usage](#usage))
 - observe DOM changes:
  - Update your code by just updating Element's text content
  - Change Editor's setting by changing DOM [attributes](#attributes)
 - Compatible with Shadow DOM v0 and v1
 - Custom Elements v1 ([more](#web-components-v0-vs-v1))

You can still fiddle with Ace editor programmatically using `<juicy-ace-editor>.editor`.

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install juicy-ace-editor --save
```

Or [download as ZIP](https://github.com/juicy/juicy-ace-editor/archive/master.zip).

## Usage

1. Import Web Components' polyfill (if needed):

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    <!-- CE v0 -> v1 -->
    <script src="document-register-element/document-register-element.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/juicy-ace-editor/juicy-ace-editor.html">
    ```

3. Start using it!

   <!--
   ```
   <custom-element-demo>
     <template>
       <script src="../webcomponentsjs/webcomponents.js"></script>
       <link rel="import" href="juicy-ace-editor.html">
       <next-code-block></next-code-block>
     </template>
   </custom-element-demo>
   ```
   -->

  ```html
  <juicy-ace-editor theme="ace/theme/monokai">Type your code here...</juicy-ace-editor>
  ```

## Attributes

Attribute  | Options   | Default | Description
---        | ---       | ---     | ---
`theme`    | *String*  |         | `Editor#setTheme` at [Ace API](http://ace.c9.io/#nav=api&api=editor)
`mode`     | *String*  |         | `EditSession#setMode` at [Ace API](http://ace.c9.io/#nav=api&api=edit_session)
`fontsize` | *String*  |         | `Editor#setFontSize` at [Ace API](http://ace.c9.io/#nav=api&api=editor)
`softtabs` | *Boolean* |         | `EditSession#setUseSoftTabs()` at [Ace API](http://ace.c9.io/#nav=api&api=edit_session)
`tabsize`  | *Boolean* |         | `Session#setTabSize()` at [Ace API](http://ace.c9.io/#nav=api&api=edit_session)
`readonly` | *Boolean* |         | `Editor#setReadOnly()` at [Ace API](http://ace.c9.io/#nav=api&api=editor)
`wrapmode` | *Boolean* |         | `Session#setWrapMode()` at [Ace API](http://ace.c9.io/#nav=api&api=edit_session)

## Properties

Name        |  Description
---         | ---
`editor`    | Ace [editor](http://ace.c9.io/#nav=api&api=editor) object.
`value`     | [editor.get-/setValue()](http://ace.c9.io/#nav=api&api=editor)

## Events

Name           |  Description
---            | ---
`change`       | Triggered when editor content gets changed
`editor-ready` | Triggered once Ace editor instance is created.

## Web Components v0 vs v1

Currently, this element supports both Shadow DOM v1 and v0, but only Custom Elements v1.
If your environment uses Custom Elements v0 only, we strongly recommend to use lightweight v0 to v1 [polyfill](https://github.com/WebReflection/document-register-element)
```sh
bower install --save document-register-element
```

## Who uses it?

- [**Starcounter** In-memory application engine](http://starcounter.com/)
- [**LEAN** Theorem prover by Microsoft Research](https://leanprover.github.io/)
- [**Polymer/polyup** Polymer migration tool](http://polymerlabs.github.io/polyup/)
- [**You** ...?](https://github.com/Juicy/juicy-ace-editor/edit/master/README.md#L107)


## [Contributing and Development](CONTRIBUTING.md)

## History

For detailed changelog, check [Releases](https://github.com/PuppetJs/redirect/releases).

## License

MIT
