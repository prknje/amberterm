# amberterm

A minimal, monospaced, terminal style theme for Hugo.

amberterm is based on [smol](https://github.com/colorchestra/smol) which is based on [Blank](https://github.com/Vimux/Blank) created by [Vimux](https://github.com/Vimux).


![Screenshot](/images/screenshot.png)

## Installation

In your Hugo site `themes` directory, run:

```
git submodule add https://git.qrz.is/clemens/amberterm
```

Next, open `config.toml` in the base of the Hugo site and ensure the theme option is set to `amberterm`.

```
theme = "amberterm"
```

Lastly, add the following lines to your `config.toml` to set site parameters and make use of all the menu entries in the header and footer sections if you need them.

```
# Parameters
[params]
    subtitle = "Your blog subtitle goes here!"
    dateFmt = "02.01.2006 15:04"

# Header
[menu]
  [[menu.main]]
        identifier = "posts"
        name = "Posts"
        url = "/posts/"
        weight = 1 

  [[menu.main]]
        identifier = "categories"
        name = "Categories"
        url = "/categories/"
        weight = 2 

  [[menu.main]]
        identifier = "tags"
        name = "Tags"
        url = "/tags/"
        weight = 3

# Footer
  [[menu.footer]]
        name = "Github"
        url = "https://github.com/example"
        weight = 1 

    [[menu.footer]]
        name = "Mastodon"
        url = "https://example.com/@user"
        weight = 2 

    [[menu.footer]]
        name = "Imprint"
        url = "/imprint"
        weight = 3 

```

For more information read the official [quick start guide](https://gohugo.io/getting-started/quick-start/) of Hugo.

## Optional features
### Custom copyright text
Add `copyright = "Your text here"` - in the config.toml to change the copyright notice in the footer.

### Image captions
You can add captions to images (technically using `<figcaption>` HTML tags) by adding titles, like so: `![Alt text here](/path/to/image.png "Put your caption here!")`

## License

This theme is released under the [MIT license](https://git.qrz.is/clemens/amberterm/raw/branch/master/LICENSE.md).
