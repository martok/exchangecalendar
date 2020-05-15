## Introduction

Exchange Calendar is an add-on for [Thunderbird](https://mozilla.org/thunderbird)
and [Seamonkey](https://www.seamonkey-project.org/).

It extends the [Lightning](https://addons.mozilla.org/thunderbird/addon/lightning/) add-on to provide
[Microsoft Exchange](http://microsoft.com/exchange) support.

Exchange Calendar extension can:
  * Synchronize calendars, tasks, and contacts with a Microsoft Exchange server.
  * Create, edit and update events and tasks.
  * Display contacts from your address books and the global address list
    (they are only readable, they are usable with address autocompletion).
  * Manage the Exchange « out of office » feature.

This extension requires:
  * A Thunderbird version from 52 up to 59 (inclusive).
  * Lightning extension corresponding to the Thunderbird release.
  * The targeted Exchange server has to provide an Exchange Web Service (EWS).

This extension was developed by its original author (Michel Verbraak) for
Exchange 2007, 2010 and 2013. It is known to work with Exchange 2016.

## Installation
Download a pre-built release from our [releases page](https://github.com/martok/exchangecalendar/releases)
or build your own release as shown below.

## Development status

This version is a continuation of development specifically for pre-Quantum versions of Thunderbird.
It will never be updated to Webextension versions of Thunderbird.

Exchange Calendar is open source and made possible by the work of many [contributors](https://github.com/ExchangeCalendar/exchangecalendar/graphs/contributors).

That project was a community driven effort to develop and maintain the
"Exchange EWS Provider" extension originally created by Michel Verbraak.

## Contributing

### Provide feedback, report issue

Please report any issues that have not previously been reported
[here](https://github.com/martok/exchangecalendar/issues). Please also check [upstream](https://github.com/ExchangeCalendar/exchangecalendar/issues).

Feel free to create issues for requests for backports or links to issues from the upstream project.

### Get project and build it

To build the add-on, you have to:
```bash
# clone this project
git clone https://github.com/ExchangeCalendar/exchangecalendar.git
cd exchangecalendar
# build it
make build
```
Then an `xpi` file is created in the project folder.
This file is directly installable from the add-on page of Thunderbird.

If it doesn't work, please check you have these tools installed (example for
Debian):
```bash
sudo apt install git-core zip
```

### Patch the code

To help us to maintain the code, we will be thankful to follow these main
guidelines:

* Use indentation with 4 spaces
* Avoid too long lines, try to break long lines into smaller ones
* Avoid to write "spaghetti" code with too many if/else imbrications
* Try to keep code simple to help us maintain it on long term

Note that our `Makefile` has a `beautify` target which will try to beautify
all JavaScript (requires `jsbeautifier` Debian package) and XML code
(requires `tidy` package) to help maintain a clean code.

When your patches are ready, you are welcome to do pull requests on our
repository.

Please help us to review your code by making multiple small pull
requests instead of big ones modifying big parts of the code.


## License

This software is provided on a best-effort basis without any warranty.
Please see the [license](http://www.gnu.org/licenses/gpl.html)
for details.

Some of the icons and images used are from the Fugue Icons Collection made
by [Yusuke Kamiyamane](http://p.yusukekamiyamane.com/).
