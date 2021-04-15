<h1 align="center">NNB's sed script collections</h1>
<p align="center">The most ambitious sed script collections</p>
<p align="center"><a href="https://github.com/NNBnh/sed-collections/watchers"><img src="https://img.shields.io/github/watchers/NNBnh/sed-collections?labelColor=585858&color=F7CA88&style=flat-square"></a> <a href="https://github.com/NNBnh/sed-collections/stargazers"><img src="https://img.shields.io/github/stars/NNBnh/sed-collections?labelColor=585858&color=F7CA88&style=flat-square"></a> <a href="https://github.com/NNBnh/sed-collections/network/members"><img src="https://img.shields.io/github/forks/NNBnh/sed-collections?labelColor=585858&color=F7CA88&style=flat-square"></a> <a href="https://github.com/NNBnh/sed-collections/issues"><img src="https://img.shields.io/github/issues/NNBnh/sed-collections?labelColor=585858&color=F7CA88&style=flat-square"></a></p>

## 💡 About
This is a collection of [`sed scripts`](https://en.wikipedia.org/wiki/Sed) to help you [filter text files](https://en.wikipedia.org/wiki/Filter_(software)).

## ⌨️ Usage
Just simply use [file-based sed scripts command](https://en.wikipedia.org/wiki/Sed#File-based_sed_scripts):

```sh
sed -f path/to/sed-file.sed path/to/text-file
```

Examples:

- Convert [emoji shortcodes](https://emojipedia.org/shortcodes) to real emojis:
```sh
sed -f path/to/sed-collections/shortcodes/emoji.sed -i path/to/text-file
```

- Roll a dice:
```sh
echo :dice_{1,2,3,4,5,6}: | sed -f path/to/sed-collections/shortcodes/dice.sed | tr ' ' '\n' | shuf | head -n 1
```

- Pick cards:
```sh
echo :card_{a,2,3,4,5,6,7,8,9,10,j,q,k}{h,d,c,s}: | sed -f path/to/sed-collections/shortcodes/card.sed | tr ' ' '\n' | shuf | more -n 1
```

<br><br><br><br>

---

> <h1 align="center">Made with ❤️ by <a href="https://github.com/NNBnh"><i>NNB</i></a></h1>
>
> <p align="center"><a href="https://www.buymeacoffee.com/nnbnh"><img src="https://img.shields.io/badge/buy_me_a_coffee%20-%23F7CA88.svg?logo=buy-me-a-coffee&logoColor=333333&style=for-the-badge" alt="Buy Me a Coffee"></p>
