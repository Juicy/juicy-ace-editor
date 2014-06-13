# &lt;tomalec-ace-editor&gt;

> Even <strong>more</strong> embeddable code editor. 
> Custom Element - just one tag, and no JS needed to provide 
> [Ace](http://ace.c9.io/) - The High Performance Code Editor

## Demo

[Check it live!](http://tomalec.github.io/tomalec-ace-editor)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install tomalec-ace-editor --save
```

Or [download as ZIP](https://github.com/tomalec/tomalec-ace-editor/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.3.2/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/tomalec-ace-editor/src/tomalec-ace-editor.html">
    ```

3. Start using it!

    ```html
    <tomalec-ace-editor></tomalec-ace-editor>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`theme`        | *string*    | ``        | See [Ace API](http://ace.c9.io/#nav=api)
`mode`         | *string*    | ``        | See [Ace API](http://ace.c9.io/#nav=api)
`fontsize`     | *string*    | ``        | See [Ace API](http://ace.c9.io/#nav=api)

## Properties

Name        |  Description
---           | ---
`editor`   | Ace [editor](http://ace.c9.io/#nav=api&api=editor) object.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/tomalec/tomalec-ace-editor/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
