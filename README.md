# cambd-cli

> [Cambridge dictionary](https://dictionary.cambridge.org) cli app for personal use

![cambd-demo-2](https://user-images.githubusercontent.com/33410545/201540858-14ba4ef5-fd96-4da6-b089-046b7440efbb.gif)

## Why

This is a personal project I have been developing and using for a while. The reason is that the only dictionary I use is the [Cambridge dictionary](https://dictionary.cambridge.org/). It has very concise and very easy-to-understand definitions. And I often find myself going back to their site in search of definitions of new words I come across daily, so I made this CLI tool to automate the process.

## Features

- Autosuggest related words if I mistyped the word when looking it up.
- Interactive suggestion menu to select words from in the above case.
- Handles past and past-particle words. Returns the original word definition.
- No API/database involved.
- Caching mechanism; so that already looked up words does not gets fetched again. Hence fast results.

> By default it caches the words in `$HOME/.cambd-cache.json`. To clear the cache if needed <br/> run `cambd --clear-cache`. It is strongly recommended to not modify this file manually.

## Installation

Make sure you have GNU `make` and `python(v3)` installed on your system.

```sh
# clone the repo
$ git clone https://github.com/rocktimsaikia/cambd-cli.git

# change the working directrory to cambd-cli
$ cd cambd-cli

# install the requirements
$ python3 -m pip install -r requirements.txt

# install cambd-cli
$ sudo make install
```

Then you can use it like this:

```sh
cambd neccesseery
```

> The above word spelling is incorrect. So cambd will suggest related words.

## TODO:

- [x] Add loading animation.
- [x] Handle error for getting definition of words with spaces.
- [x] Show only 2 examples per definition by default.
- [x] Implement a basic local caching mechanism.
- [x] Handle past/past-participle word definitions.
- [x] Refactor redirection for better word lookup.
- [ ] Better/clean way to print the values in terminal.
- [ ] Add flag to show all definitions. Default is 1.

## LICENSE

[MIT](./LICENSE) License &copy; [Rocktim Saikia](https://rocktimsaikia.com) 2022
