# Contributing

Hi there! We are thrilled that you would like to contribute to this project. Your help is essential for keeping it great.

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change.
If an issue is opened and more info is needed, `airgeddon` staff will request it. If there is no answer in 7 days, the issue will be closed. Issues must be opened in english.

Please note we have a [Code of Conduct], please follow it in all your interactions with the project.

---

## Collaborating Translators

1. Update the date under shebang.
2. Translate the strings located in `language_strings.sh` and the existing phrases _language_strings_handling_messages function_ in `airgeddon.sh`.
3. Ask by mail [v1s1t0r.1s.h3r3@gmail.com] if you have any doubt. You'll be informed about how to proceed.
4. You can be added as a collaborator on the project.
5. Knowledge about `git` is not mandatory but is really appreciated to push directly into the project repository.
6. If you want to create a pull request with a new language to be added, at least the 80% of the phrases must be translated and the rest must be done with at least _an automatic-translation_ system and marked with PoT (Pending of Translation) mark.

## Collaborating Developers

1. Tweak *"debug_mode"* variable to "1" for faster development skipping intro and initial checks or to "2" for verbosity and the skips mentioned before.
2. Respect the **4 width tab indentation**, code style and the **UTF-8 encoding**.
3. Use **LF** (Unix) line break type (not CR or CRLF).
4. Use [Shellcheck] to search for errors and warnings on code. (Thanks [xtonousou] for the tip :wink:). To avoid false positive warnings you must launch shellcheck using `-x` argument to follow source files and from the directory where `airgeddon.sh` is. For example: `cd /path/to/airgeddon && shellcheck -x airgeddon.sh`
5. Increase the version numbers in `airgeddon.sh`, in [Readme] and in [Changelog] to the new version that the script represents. The versioning scheme we use is *X.YZ*. Where:
  - *X* is a major release with a new menu (e.g. WPS menu)
  - *Y* is a minor release with a new feature for an existing menu or a new submenu for an existing feature
  - *Z* is a minor release with new bug fixes, small modifications or code improvements
6. Update the date on `.sh` and `.db` files under shebang, if appropriate.
7. Split your commits into parts. Each part represents a unique change on files.
8. Direct push to [Master] is not allowed.
9. Pull Requests to [Master] are not allowed. Should be done over [Dev] or any other branch. They require revision and approvement.
10. All the development and coding must be in English.

*Be sure to merge the latest from "upstream" before making a pull request!*

We also have a private Telegram group for *trusted collaborators* for more agile discussion about developments, improvements, etc. 
To be added on it you must prove first you are a *trusted collaborator* with your contributions.

## WPS PIN Database Collaborators

1. Send MAC of the BSSID and the default PIN to [v1s1t0r.1s.h3r3@gmail.com]. If you are going to push directly into the repository, keep reading the next points.
2. Add PINs ordered by the key in the associative array located in the `known_pins.db` file. (Keys are the first 6 BSSID digits).
3. Update the `pindb_checksum.txt` file with the calculated checksum of the database file using `md5sum` tool.
4. Update the date under shebang.

*PINs should be from devices that generate generic ones.*

## Beta Testers

1. Download the master version or the beta testing version from the development branch called [Dev]. Temporary branches may be existing for specific features that can be tested too.
2. Report any issues or bugs by mail [v1s1t0r.1s.h3r3@gmail.com] or submit issue requests [Here].

---

## Donate

If you enjoyed the script, feel free to donate. Support the project through Paypal or sending a fraction any of these cryptocurrencies. Any amount, not matter how small (1, 2, 5 $/€) is welcome:

<table>
  <tr>
    <td>
      <b>Paypal</b>: <em>v1s1t0r.1s.h3r3&#64;gmail.com</em> <br/>
      <b>Bitcoin</b>: <em>1NSzwqtBBdo4CrvynPZmd85xfbL7hw3Ptu</em> <br/>
      <b>Bitcoin Cash</b>: <em>1GyUesBgwHKZBeFvkT5nfteecPdH6bAEaL</em> <br/>
      <b>Dash</b>: <em>XgKL8GTsdKAL2fypiMRFFL8m4wWTm1Netn</em> <br/>
      <b>Ethereum</b>: <em>0xf88107ba5e10776a37ec089a7ed2bac57638eea7</em> <br/>
      <b>Litecoin</b>: <em>LX1ytoQhRzUAuArpkNRjnfTmwYuxxJezTn</em> <br/>
      <b>ZCash</b>: <em>t1dt1ZDCgDUt9pqnyzkZd9GE2NpZBfMVsXq</em>
    </td>
  </tr>
</table>

<br/>

<div align="center">
    <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7ELM486P7XKKG"><img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/paypal_donate.png" title="Paypal"/></a>
</div>

<br/>

<div align="center">
  <table>
    <tr>
      <td>
        Bitcoin QR code:
      </td>
      <td>
        Bitcoin Cash QR code:
      </td>
      <td>
        Dash QR code:
      </td>
    </tr>
    <tr>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/bitcoin_qr.png" title="Bitcoin"/>
      </td>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/bitcoincash_qr.png" title="Bitcoin Cash"/>
      </td>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/dash_qr.png" title="Dash"/>
      </td>
    </tr>
    <tr>
      <td>
        Ethereum QR code:
      </td>
      <td>
        Litecoin QR code:
      </td>
      <td>
        ZCash QR code:
      </td>
    </tr>
    <tr>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/ethereum_qr.png" title="Ethereum"/>
      </td>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/litecoin_qr.png" title="Litecoin"/>
      </td>
      <td>
        <img src="https://raw.githubusercontent.com/v1s1t0r1sh3r3/airgeddon/master/imgs/banners/zcash_qr.png" title="ZCash"/>
      </td>
    </tr>
  </table>
</div>

<!-- MDs -->
[Readme]: README.md
[Changelog]: CHANGELOG.md
[Code of Conduct]: CODE_OF_CONDUCT.md

<!-- Github -->
[Shellcheck]: https://github.com/koalaman/shellcheck "shellcheck.hs"
[Here]: https://github.com/v1s1t0r1sh3r3/airgeddon/issues/new
[Master]: https://github.com/v1s1t0r1sh3r3/airgeddon/tree/master
[Dev]: https://github.com/v1s1t0r1sh3r3/airgeddon/tree/dev
[xtonousou]: https://github.com/xtonousou "xT"
