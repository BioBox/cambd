# cambd-cli

> Cambridge dictionary cli app for my personal use

https://user-images.githubusercontent.com/33410545/201367453-1bc9f6cf-9688-4b2c-a67b-32645272eba2.mov




## Why

This is a personal project I have been developing and using for a while. The reason is that the only dictionary I use is the [Cambridge dictionary](https://dictionary.cambridge.org/). It has very concise and very easy-to-understand definitions. And I often find myself going back to their site in search of definitions of new words I come across daily, so I made this CLI tool to automate the process.

I only want two things from my CLI

1. I always spell words wrong while typing. In that case suggest me the correct word or related words.
2. If the provided word is spelled correctly then give the defination with minimum examples.

THAT's all!

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

## Uninstall

To uninstall you can run the below command from the `cambd-cli` directory

```sh
sudo make uninstall
```

## TODO:

- [x] Add loading animation
- [x] Handle error for getting definition of words with spaces
- [x] Show only 2 examples per definition by default
- [ ] Add flag to show all definitions. Default is 1

## LICENSE

[MIT](./LICENSE) License &copy; [Rocktim Saikia](https://rocktimsaikia.com) 2022
