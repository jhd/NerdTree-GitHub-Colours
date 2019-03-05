# NerdTree-GitHub-Colours

Highlight files in NerdTree using their GitHub colour.

### How to use:
* Save `nerdtree-github-colours.vim` file in your `~/.vim/colors/`.
* Add `source ~/.vim/colors/nerdtree-github-colours.vim` to your `.vimrc`.
* Enable any non-default extensions you use. (Make sure to uncomment both the syn match line and the hightlight line).

### Screenshots

![](/screenshots/dark.png)
![](/screenshots/light.png)

### FAQ
#### How does this handle term colours (8-bit)?
I use an 8-bit approximation of the RGB colours. The results are very similar.

#### Why aren't all of the colours enabled by default?
Vim's highlighting can't really handle more than 70 extensions without lagging horribly, and GitHub supports 644 extensions. Seriously there are like 30 different lisp extensions. I just enabled the most common ones by default. 

#### Why are some colours hard to read on a dark background?
GitHub's colours were made for display on the white background of their site, some of the colours may be hard to read on very dark backgrounds. On my gray background (#272822) all of the default colours are readable.

#### This script makes NerdTree laggy for me.
Disable (comment) some of the extensions, both the syn match line and the highlight line.

#### My extension isn't highlighted.
Check that the extension is enabled in the `nerdtree-github-colours.vim` file. If its not there at all GitHub doesn't recognise your extension, you can raise it with the [here](https://github.com/github/linguist/blob/master/CONTRIBUTING.md#adding-an-extension-to-a-language).
