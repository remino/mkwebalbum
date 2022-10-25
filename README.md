mkwebalbum
==========

By Rémino Rem <https://remino.net/>

Create .htaccess file for Apache HTTPd to show a stylised directory index.

[Code & Download](https://github.com/remino/mkwebalbum/)

- [Getting Started](#getting-started)
	- [Prerequisites](#prerequisites)
	- [Installation](#installation)
		- [Using Homebrew on macOS](#using-homebrew-on-macos)
		- [Using git](#using-git)
		- [Using cURL](#using-curl)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)



## Getting Started

### Prerequisites

- awk
- [Imagemagick](https://imagemagick.org/index.php)

### Installation

#### Using Homebrew on macOS

```sh
brew tap remino/remino
brew install mkwebalbum
mkwebalbum -h
```
#### Using git

```sh
git clone https://github.com/remino/mkwebalbum.git
cd mkwebalbum
./mkwebalbum -h
```

#### Using cURL

```sh
curl -L https://github.com/remino/mkwebalbum/raw/main/mkwebalbum > mkwebalbum
chmod +x mkwebalbum
./mkwebalbum -h
```

[Back to top](#mkwebalbum)



## Usage

```
mkwebalbum 1.3.0

USAGE: mkwebalbum [<options>] [<inputdir>] [<outputfile>]

Generate album Web page with previews from a directory of photos.

Only the top-level directory is processed and only the image files are listed
by default. Dot files and directories are ignored. If <inputdir> is not given,
the current directory is used.

Outputs to index.html by default unless specified otherwise. Can also output to
stdout if <outputfile> is specified as '-'.

Requires awk and imagemagick.

OPTIONS:

	-a          List all files and sub-directions.
	-e <regex>  Exclude files with name matching this regex.
	            Defaults to '^\.'.
	-h          Show this help screen.
	-r          Regenerate previews instead of skipping those that already exist.
	-t <title>  Specify HTML title. Defaults to name of <inputdir>.
	-v          Show script name and version number.

```

[Back to top](#mkwebalbum)



## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

[Back to top](#mkwebalbum)



## License

Distributed under the ISC License. See `LICENSE.txt` for more information.

[Back to top](#mkwebalbum)
