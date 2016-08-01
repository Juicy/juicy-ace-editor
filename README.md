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

You can still fiddle with Ace editor programmatically using `<juicy-ace-editor>.editor`.

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install juicy-ace-editor --save
```

Or [download as ZIP](https://github.com/juicy/juicy-ace-editor/archive/gh-pages.zip).

## Usage

1. Import Web Components' polyfill (if needed):

    ```html
    <script src="//cdn.jsdelivr.net/webcomponentsjs/0.6.0/webcomponents.min.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/juicy-ace-editor/juicy-ace-editor.html">
    ```

3. Start using it!

    ```html
    <juicy-ace-editor>Editable code here</juicy-ace-editor>
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

## Who uses it?

- [**Starcounter** In-memory application engine](http://starcounter.com/)
- [**LEAN** Theorem prover by Microsoft Research](https://leanprover.github.io/)
- [**Polymer/polyup** Polymer migration tool](http://polymerlabs.github.io/polyup/)
- [**You** ...?](https://github.com/Juicy/juicy-ace-editor/edit/gh-pages/README.md#L81)


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D


## History

For detailed changelog, check [Releases](https://github.com/PuppetJs/redirect/releases).

## License

MIT
