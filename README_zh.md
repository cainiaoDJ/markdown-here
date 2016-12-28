# ![Markdown Here logo](https://raw.github.com/adam-p/markdown-here/master/src/common/images/icon48.png) Markdown Here

*约定：*  本人将`Markdown Here`翻译为『马克飞呀』，下同 

[**访问我们的网站.**](http://markdown-here.com)  
[**获取 Chrome 版本**](https://chrome.google.com/webstore/detail/elifhakcjgalahccnjkneoccemfahfoa)  
[**获取 Firefox 版本**](https://addons.mozilla.org/en-US/firefox/addon/markdown-here/)  
[**获取 Safari 版本**](https://s3.amazonaws.com/markdown-here/markdown-here.safariextz)  
[**获取 Thunderbird 和 Postbox版本**](https://addons.mozilla.org/en-US/thunderbird/addon/markdown-here/)  
[**获取 Opera 版本**](https://addons.opera.com/en/extensions/details/markdown-here/)  
[**在谷歌团队协作中讨论和咨询**](https://groups.google.com/forum/?fromgroups#!forum/markdown-here/)

*Markdown Here* 是一个 Google Chrome, Firefox, Safari, Opera, 和 Thunderbird 中的插件，方便你在写邮件时使用Markdown语法，而且在发送之前可以预览. 与此同时他还支持语法高亮 （只需在代码区域内添加代码块）。

写含有代码块的邮件是一件非常痛苦的事，而用Markdown是很容易的一件事。 我发现自己在Github的浏览器编辑器中用Markdown写电子邮件，然后将预览复制到电子邮件中。 这是一个非常可笑的工作流，所以我决定创建一个工具，在电子邮件中写入和渲染Markdown。

要探索在*Markdown Here*中可以用Markdown做些什么，可以检出这个[Markdown Here Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet) 和另外的[Wiki页面](https://github.com/adam-p/markdown-here/wiki)。

<sup>&dagger;: And Google Groups posts, and Blogger posts, and Evernote notes, and Wordpress posts! [See more](#compatibility).</sup>  
<sup>&Dagger;: And TeX mathematical formulae!</sup>

![screenshot of conversion](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image1.gimp.png)

### 目录
**[安装说明](#installation-instructions)**  
**[使用说明](#usage-instructions)**  
**[故障排除](#troubleshooting)**  
**[兼容性](#compatibility)**  
**[注释和杂项](#notes-and-miscellaneous)**  
**[构建扩展包](#building-the-extension-bundles)**  
**[后续计划，贡献，反馈，许可证](#next-steps)**  

## 安装说明

### Chrome

#### Chrome 应用商店

访问 [Chrome 应用商店中的 *Markdown Here*](https://chrome.google.com/webstore/detail/elifhakcjgalahccnjkneoccemfahfoa) and install normally.

安装完成之后，请确保重新加载邮件页面或者重新加载 Chrome 浏览器!

#### 手册/开发
*扩展可以理解为插件*
1. 克隆这个仓库。
2. 在Chrome中，打开扩展设置。（扳手按钮，工具，扩展）。
3. 在扩展设置页面， 点击选中“开发者模式”。
4. 点击刚刚出现的 『加载已解压的扩展程序...』 按钮。 导航到你刚才克隆源码的目录， 然后选中目下的`src`文件夹.
5. 现在*Markdown Here* 扩展已经就会出现在你的扩展列表了.
6. 在你准备转换邮件之前，重新加载页面(也可能是一个应用) 。

### Firefox（火狐：浏览器） and Thunderbird（雷鸟：邮件客户端）

#### Mozilla 附加组建网站

访问 [火狐附加组件中的 *Markdown Here*](https://addons.mozilla.org/en-US/firefox/addon/markdown-here/) 并且执行安装.

或者点击"工具 > 附加组件..." 菜单，然后搜索 "Markdown Here".

安装完成之后, 请确保重启了 Firefox 或 Thunderbird!

**备注：** Mozilla最长需要一个月才能批准对Firefox / Thunderbird扩展的更改, 因此更新(功能, 修复) 将会滞后于现在显示在本页面的说明。 您可以手动选择安装最新版本，然后再从版本列表中进行审核: [https://addons.mozilla.org/en-US/firefox/addon/markdown-here/versions/](https://addons.mozilla.org/en-US/firefox/addon/markdown-here/versions/)

#### 手册/开发

1. 克隆这个仓库。
2. 按照MDN中的说明操作 ["设置扩展开发环境"](https://developer.mozilla.org/en/Setting_up_extension_development_environment) 。

### Safari

[直接下载这个扩展。](https://s3.amazonaws.com/markdown-here/markdown-here.safariextz) 下载完毕后，双击安装。 

#### 偏好设置

要想设置 Markdown Here 偏好设置， 打开 *Safari偏好设置* 然后点击扩展标签页，然后点击 "Click me to show Markdown Here options" 单选框。 

### 欧朋浏览器

Note that *Markdown Here* only works with Opera versions 16 and higher (i.e., the ones that are based on Chromium).

Go to the [Opera Add-ons store page for *Markdown Here*](https://addons.opera.com/en/extensions/details/markdown-here/) and install normally.

After installing, make sure to reload your webmail or restart Chrome!

## 使用说明

Install it, and then…

1. In Chrome/Safari/Opera, *make sure* you reload your web mail page before trying to use Markdown Here.
2. In Chrome/Firefox/Safari/Opera, log into your Gmail, Hotmail, or Yahoo account and start a new email. In Thunderbird, start a new message.
3. Make sure you're using the rich editor.
   * In Gmail, click the "Rich formatting" link, if it's visible.
   * In Thunderbird, make sure "Compose messages in HTML format" is enabled in your "Account Settings", "Composition & Addressing" pane.
4. Compose an email in Markdown. For example:

   <pre>
   **Hello** `world`.

   ```javascript
   alert('Hello syntax highlighting.');
   ```
   </pre>

5. Right-click in the compose box and choose the "Markdown Toggle" item from the context menu. Or click the button that appears in your address bar. Or use the hotkey (<kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>M</kbd> by default).
6. You should see your email rendered correctly from Markdown into rich HTML.
7. Send your awesome email to everyone you know. It will appear to them the same way it looks to you.

### Revert to Markdown

After rendering your Markdown to pretty HTML, you can still get back to your original Markdown. Just right-click anywhere in the newly rendered Markdown and click "Markdown Toggle" -- your email compose body will change back to the Markdown you had written.

Note that any changes you make to the pretty HTML will be lost when you revert to Markdown.

In Gmail, you can also use the browser's Undo command (<kbd>CTRL</kbd>+<kbd>Z</kbd> / <kbd>CMD</kbd>+<kbd>Z</kbd>, or from the Edit menu). Be warned that you might also lose the last few characters you entered.

### Replies

In Gmail, Thunderbird, and Google Groups, you can use "Markdown Toggle" normally: just write your reply (top, bottom, inline, wherever) and then convert. The original email that you're replying to will be left alone. (Technically: Existing `blockquote` blocks will be left intact.) 

In Hotmail and Yahoo (which don't put the original in a `blockquote`), and optionally in Gmail, Thunderbird, and Google Groups, you can ensure that only the part of the reply that you wrote gets converted by selecting what you want to convert and then clicking "Markdown Toggle" -- see the next section.

### Selection/Piecemeal Conversion

Sometimes you don't want to convert the entire email; sometimes your email isn't entirely Markdown. To convert only part of the email, select the text (with your mouse or keyboard), right-click on it, and click the "Markdown Toggle" menu item. Your selection is magically rendered into pretty HTML.

To revert back to Markdown, just put your cursor anywhere in the block of converted text, right click, and click the "Markdown Toggle" menu item again. Now it's magically back to the original Markdown.

![screenshot of selection conversion](https://raw.github.com/adam-p/markdown-here/master/store-assets/markdown-here-image2.gimp.png)

#### Things to know about converting/reverting a selection

* If you select only part of a block of text, only that text will be converted. The converted block will be wrapped in a paragraph element, so the original line will be broken up. You probably don't want to ever do this.

* You can select and revert multiple converted blocks at the same time. One upshot of this is that you can select your entire email, click "Markdown Toggle", and all portions of it that you had converted will be reverted.

* If you don't have anything selected when you click "Markdown Toggle", *Markdown Here* will check if there are converted blocks anywhere in the message and revert them. If there no converted blocks are found, it will convert the entire email.

### Options

The *Markdown Here* Options page can be accessed via the Chrome, Firefox, Safari, or Thunderbird extensions list. The available options include:

* Styling modifications for the rendered Markdown.
* Syntax highlighting theme selection and modification.
* TeX math formulae processing enabling and customization.
* What the hotkey should be.

For Chrome and Firefox, any changes made in the *Markdown Here* Options are automatically synchronized between your other installations of that browser (if you have the sync feature enabled in the browser). 

![screenshot of options](https://raw.githubusercontent.com/adam-p/markdown-here/master/store-assets/markdown-here-chrome-options-1.gimp.png)


## Troubleshooting

See the [Troubleshooting wiki page](https://github.com/adam-p/markdown-here/wiki/Troubleshooting).


## Compatibility

See the [Compatibility wiki page](https://github.com/adam-p/markdown-here/wiki/Compatibility).


## Notes and Miscellaneous

* *Markdown Here* uses [Github Flavored Markdown](http://github.github.com/github-flavored-markdown/), with the limitation that GFM special links are not supported ([issue #11](https://github.com/adam-p/markdown-here/issues/11)); nor will they be, as MDH is not Github-specific.

* Available languages for syntax highlighting (and the way they should be written in the fenced code block) can be seen on the [highlight.js demo page](http://softwaremaniacs.org/media/soft/highlight/test.html).

* Images embedded inline in your Markdown will be retained when you "Markdown Toggle". Gmail allows you to put images inline in your email -- this can be much easier than referencing an external image.

* Email signatures are automatically excluded from conversion. Specifically, anything after the semi-standard `'-- '` (note the trailing space) is left alone.
  * Note that Hotmail and Yahoo do *not* automatically add the `'-- '` to signatures, so you have to add it yourself.

* The "Markdown Toggle" menu item shows up for more element types than it can correctly render. This is intended to help people realize that they're not using a rich editor. Otherwise they just don't see the menu item and don't know why.

* Styling:
  * The use of browser-specific styles (-moz-, -webkit-) should be avoided. If used, they may not render correctly for people reading the email in a different browser from the one where the email was sent.
  * The use of state-dependent styles (like `a:hover`) don't work because they don't match at the time the styles are made explicit. (In email, styles must be explicitly applied to all elements -- stylesheets get stripped.)

* For more tweaky features, visit the [Tips and Tricks](https://github.com/adam-p/markdown-here/wiki/Tips-and-Tricks) section.

## Building the Extension Bundles

"Building" is really just zipping. Create all archives relative to the `src` directory.

Before zipping, delete the `src/common/test` directory. This will prevent the autotests from ending up in the release.

An important preparatory step is to remove any system-generated hidden files that shouldn't be 
included in the release file (like Windows' `desktop.ini` and OS X's `.DS_Store`, etc.). This shell command will delete those unwanted files: 

```
find . -name "desktop.ini" -or -name ".*" -and -not -name "." -and -not -name ".git*" -print0 | xargs -0 rm -rf
```

### Chrome and Opera extension

Create a file with a `.zip` extension containing these files and directories:

```
manifest.json
common/
chrome/
```

### Firefox/Thunderbird extension

Create a file with a `.xpi` extension containing these files and directories:

```
chrome.manifest
install.rdf
common/
firefox/
```

### Safari extension

The browser-specific code is located in the [`markdown-here-safari`](https://github.com/adam-p/markdown-here-safari) project.

Use the Safari Extension Builder.

## Next Steps

See the [issues list](https://github.com/adam-p/markdown-here/issues) and the [Notes Wiki](https://github.com/adam-p/markdown-here/wiki/Development-Notes). All ideas, bugs, plans, complaints, and dreams will end up in one of those two places.

Feel free to create a feature request issue if what you want isn't already there. If you'd prefer a less formal approach to floating an idea, post to the ["markdown-here" Google Group](https://groups.google.com/forum/?fromgroups=#!forum/markdown-here).

It also takes a fair bit of work to stay up-to-date with the latest changes in all the applications and web sites where Markdown Here works.

## Credits

*Markdown Here* was coded on the shoulders of giants.

* Markdown-to-HTML: [chjj / marked](https://github.com/chjj/marked)
* Syntax highlighting: [isagalaev / highlight.js](https://github.com/isagalaev/highlight.js)
* HTML-to-text: [mtrimpe / jsHtmlToText](https://github.com/mtrimpe/jsHtmlToText)

## Feedback

All bugs, feature requests, pull requests, feedback, etc., are welcome. [Create an issue](https://github.com/adam-p/markdown-here/issues). Or [post to the "markdown-here" Google Group](https://groups.google.com/forum/?fromgroups=#!forum/markdown-here).

## License

### Code

MIT License: http://adampritchard.mit-license.org/ or see [the `LICENSE` file](https://github.com/adam-p/markdown-here/blob/master/LICENSE).

### Logo

Copyright 2015, [Austin Anderson](http://protractor.ninja/). Licensed to Markdown Here under the [MDH contributor license agreement](https://github.com/adam-p/markdown-here/blob/master/CLA-individual.md).

### Other images

[Creative Commons Attribution 3.0 Unported (CC BY 3.0) License](http://creativecommons.org/licenses/by/3.0/)

---

![Dos Equis man says](https://raw.github.com/adam-p/markdown-here/master/store-assets/dos-equis-MDH.jpg)
