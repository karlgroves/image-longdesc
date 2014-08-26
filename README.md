# &lt;image-longdesc&gt;

> Adds image alt text as a caption for the image and adds a longdesc link

What's longdesc?  Well, other than being a controversial HTML attribute, it is intended to contain a URI at which a user
can get a full description of the content conveyed by an image. Read this: [http://www.w3.org/TR/2014/CR-html-longdesc-20140812/](http://www.w3.org/TR/2014/CR-html-longdesc-20140812/)

## Demo

[Check it live!](http://karlgroves.github.io/image-longdesc)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install image-longdesc --save
```

Or [download as ZIP](https://github.com/karlgroves/image-longdesc/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/image-longdesc/dist/image-longdesc.html">
    ```

3. Start using it!

    ```html
    <image-longdesc src="/foo.png" alt="useful alt for the foo image"></image-longdesc>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`src`         | *string*    | blank        | the source file for the image
`alt`         | *string*    | blank        | the alt attribute for the image
`longdesc`    | *string*    | blank        | valid URI for a long description of the image

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/karlgroves/image-longdesc/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
