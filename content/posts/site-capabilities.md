+++
title = "Testing the Site's Capabilities"
date = "2024-01-02"
description = "Testing my Theme and Capabilities of my Site. Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags = [
    "markdown",
    "syntax",
    "testing"
]
author = "Varsh"
+++

For a quick cheatsheet, check out https://simplemde.com/markdown-guide.

{{< tellblock note >}}

🏗️🚧 This post is just a dummy post to test this Site's Capabilities

{{< /tellblock >}}

---

{{< tocblock >}}

---



This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.
<!--more-->


## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is {{< htmlblock >}}
<svg xmlns="http://www.w3.org/2000/svg" width="1rem" height="1rem" viewBox="0 0 24 24"><path fill="currentColor" d="M20.664 5.253a1 1 0 0 1 .083 1.411l-10.666 12a1 1 0 0 1-1.495 0l-5.333-6a1 1 0 0 1 1.494-1.328l4.586 5.159l9.92-11.16a1 1 0 0 1 1.411-.082"/></svg>
{{</ htmlblock >}} the highest section level while `<h6>` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.
> <br> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

> Quote1
>
> Quote2

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

   Name | Age | Hi | How | meow | Lol | horo | hora | toha
--------|------|----|-----|-----| --- | --- | --- | ---
    Bob | 27   | 33 | 44 | 55 | 2222222| 22 | 555 | 22222
  Alice | 23 | 44 | 22 | 22 | hoarci | hora | ora | oba


{{< htmlblock >}}
<br>
<code>Hello</code>
<br>
{{</ htmlblock >}}




{{< tellblock note >}}




{{< htmlblock >}}
<div style="display: flex; justify-content: space-between; gap: 1em"> 
<img height="55px" src="https://images.pexels.com/photos/45201/kitty-cat-kitten-pet-45201.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500"/>
  <strong>Incididunt labore eiusmod culpa eu nostrud tempor laborum consequat eiusmod excepteur.</strong>
 </div>
{{< /htmlblock >}}

  ---

Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur officia. Reprehenderit {{< htmlblock >}}
<img height="55px" class="display: inline-block;" src="https://images.pexels.com/photos/45201/kitty-cat-kitten-pet-45201.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500"/>{{< /htmlblock >}}nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.

```bash
#!/bin/bash
cd $ROOT_DIR
DOT_FILES="lastpass weechat ssh Xauthority"
for dotfile in $DOT_FILES; do conform_link "$DATA_DIR/$dotfile" ".$dotfile"; done
 
# TODO: refactor with suffix variables (or common cron values)
 
case "$PLATFORM" in
    linux)
        #conform_link "$CONF_DIR/shell/zshenv" ".zshenv"
        crontab -l > $ROOT_DIR/tmp/crontab-conflict-arch
        cd $ROOT_DIR/$CONF_DIR/cron
        if [[ "$(diff ~/tmp/crontab-conflict-arch crontab-current-arch)" == ""
            ]];
            then # no difference with current backup
                logger "$LOG_PREFIX: crontab live settings match stored "\
                    "settings; no restore required"
                rm ~/tmp/crontab-conflict-arch
            else # current crontab settings in file do not match live settings
                crontab $ROOT_DIR/$CONF_DIR/cron/crontab-current-arch
                logger "$LOG_PREFIX: crontab stored settings conflict with "\
                    "live settings; stored settings restored. "\
                    "Previous settings recorded in ~/tmp/crontab-conflict-arch."
        fi
    ;;
```

{{< /tellblock >}}
{{< tellblock info >}}
  Incididunt labore eiusmod culpa eu nostrud tempor laborum consequat eiusmod excepteur.
{{< /tellblock >}}
{{< tellblock warning >}}
  Incididunt labore eiusmod culpa eu nostrud tempor laborum consequat eiusmod excepteur.
{{< /tellblock >}}
{{< tellblock important >}}
  Incididunt labore eiusmod culpa eu nostrud tempor laborum consequat eiusmod excepteur.
| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |



```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```


{{< /tellblock >}}
{{< tellblock tip >}}
  Incididunt labore eiusmod culpa eu nostrud tempor laborum consequat eiusmod excepteur.
{{< /tellblock >}}


{{< tellblock info >}}
**This is a bold line**

Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam, omnis aliquam...
{{< /tellblock >}}

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |




## Other Sections

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.


> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

![The San Juan Mountains are beautiful!](https://raw.githubusercontent.com/makccr/wallpapers/master/wallpapers/landscape/Old%20Man%20of%20Storr.jpg "San Juan Mountains")

{{< htmlblock  >}}<details><summary>Hellllo</summary> <button>Hello</button></details> {{< /htmlblock >}}


{{< htmlblock >}}
  <figure>

<video controls width="700">
  <source src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm" type="video/webm" />

  <source src="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4" type="video/mp4" />

  Download the
  <a href="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm">WEBM</a>
  or
  <a href="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4">MP4</a>
  video.


</video>
    <figcaption>Video</figcaption>
  </figure>


<figure>
  <figcaption>Listen to the T-Rex:</figcaption>
  <audio controls src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3"></audio>
  <br>
  <a style="display:block; text-align: center" href="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3"> Download audio </a>
</figure>
{{</ htmlblock >}}


> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>



Freedom[^freedom] 

[^freedom]: Freedom citation



## Code Blocks

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Language Tests

Note: I took this test post from [moving](https://github.com/huangyz0918/moving), which is another Jekyll theme which is better that this one so I should not have linked it because now you will decide to use it instead of mine.

### 1. 日本語テスト

This is a Japanese test post to show you how japanese is displayed.

私は昨日ついにその助力家というのの上よりするたなけれ。
最も今をお話団はちょうどこの前後なかろでくらいに困りがいるたをは帰着考えたなかって、そうにもするでうたらない。
がたを知っないはずも同時に九月をいよいよたありた。

もっと槙さんにぼんやり金少し説明にえた自分大した人私か影響にというお関係たうませないが、この次第も私か兄具合に使うて、槙さんののに当人のあなたにさぞご意味と行くて私個人が小尊敬を聴いように同時に同反抗に集っだうて、いよいよまず相当へあっうからいだ事をしでなけれ。

> それでそれでもご時日をしはずはたったいやと突き抜けるますて、その元がは行ったてという獄を尽すていけですた。

この中道具の日その学校はあなたごろがすまなりかとネルソンさんの考えるですん、辺の事実ないというご盲従ありたですと、爺さんのためが薬缶が結果までの箸の当時してならて、多少の十月にためからそういう上からとにかくしましないと触れべきものたで、ないうですと多少お人達したのでたた。

From [すぐ使えるダミーテキスト - 日本語 Lorem ipsum.](http://lipsum.sugutsukaeru.jp/index.cgi) 


### 2. 繁体中文测试

This is a chinese test post to show you how chinese is displayed.

善我王上魚、產生資西員合兒臉趣論。畫衣生這著爸毛親可時，安程幾？合學作。觀經而作建。都非子作這！法如言子你關！手師也。

以也座論頭室業放。要車時地變此親不老高小是統習直麼調未，行年香一？

就竟在，是我童示讓利分和異種百路關母信過明驗有個歷洋中前合著區亮風值新底車有正結，進快保的行戰從：弟除文辦條國備當來際年每小腳識世可的的外的廣下歌洲保輪市果底天影；全氣具些回童但倒影發狀在示，數上學大法很，如要我……月品大供這起服滿老？應學傳者國：山式排只不之然清同關；細車是！停屋常間又，資畫領生，相們制在？公別的人寫教資夠。資再我我！只臉夫藝量不路政吃息緊回力之；兒足灣電空時局我怎初安。意今一子區首者微陸現際安除發連由子由而走學體區園我車當會，經時取頭，嚴了新科同？很夫營動通打，出和導一樂，查旅他。坐是收外子發物北看蘭戰坐車身做可來。道就學務。

國新故。

> 工步他始能詩的，裝進分星海演意學值例道……於財型目古香亮自和這乎？化經溫詩。只賽嚴大一主價世哥受的沒有中年即病行金拉麼河。主小路了種就小為廣不？

From [亂數假文產生器 - Chinese Lorem Ipsum.](http://www.richyli.com/tool/loremipsum/) 



### 3. 简体中文测试

效育声去本义然空，各值太法心想，场强实地。 题铁习点儿表管少间千，只何政亲织文意部，千影画派证男须。 手反取长风治增非等直难群，连取及天他己事头级，影数弦适把气快目人。 专议以省通引而千个，格则口段度样水热马，地教少务改磨。 包思外心半院应她算斯，市外会快记路又火学，劳如肃它准众丧边。
   
  > 团算部住县单总边素格军所，合音府教看和广光采率位转，位用品根确针百。 证其标元角工方海接交他，论象切万世认一响义，治然身本风弦带题。 向我次路持加北，她不反心。 说总元军例市决，现始即算证养，规走还壳。

因林可相儿应满军，热影省条律因资再，整肃赤心将届。 局广写两量备验还，南教事争工民的，备进研上布。 素身电活非直，速这区交示从，百层达。 资量那毛什京身，白这快。 半打容三手开常价或，手严量般象式效，名可重芽门适。 来设什一我么，光界美么或，住身式准。 造酸改表委验众办地百养，商物战众本列听度名院，制压录丽快与千机内。 住需当四议决得命南然照按民置，当住命形金决否矿单外。 气象理离开新集增际，三划方工义很年关，拉许准孝口。 构片出干计由备美打养，持育总指承入无己。

From [假文生成器， lorem ipsum Chinese](http://www.cancms.com/content/dummytext)

# Codeblocks



#### Test for C
```c
#define UNICODE
#include <windows.h>
 
int main(int argc, char **argv) {
  int speed = 0, speed1 = 0, speed2 = 0; // 1-20
  printf("Set Mouse Speed by Maverick\n");
 
  SystemParametersInfo(SPI_GETMOUSESPEED, 0, &speed, 0);
  printf("Current speed: %2d\n", speed);
 
  if (argc == 1) return 0;
  if (argc >= 2) sscanf(argv[1], "%d", &speed1);
  if (argc >= 3) sscanf(argv[2], "%d", &speed2);
 
  if (argc == 2) // set speed to first value
    speed = speed1;
  else if (speed == speed1 || speed == speed2) // alternate
    speed = speed1 + speed2 - speed;
  else
    speed = speed1;  // start with first value
 
  SystemParametersInfo(SPI_SETMOUSESPEED, 0,  speed, 0);
  SystemParametersInfo(SPI_GETMOUSESPEED, 0, &speed, 0);
  printf("New speed:     %2d\n", speed);
  return 0;
}
```

#### Test for Java

```java
import java.util.Map;
import java.util.TreeSet;
 
public class GetEnv {
  /**
   * let's test generics
   * @param args the command line arguments
   */
  public static void main(String[] args) {
    // get a map of environment variables
    Map<String, String> env = System.getenv();
    // build a sorted set out of the keys and iterate
    for(String k: new TreeSet<String>(env.keySet())) {
      System.out.printf("%s = %s\n", k, env.get(k));
    }
  }    
}
```

#### Test for Perl

```perl
#!perl -w
 
# Time-stamp: <2002/04/06, 13:12:13 (EST), maverick, csvformat.pl>
# Two pass CSV file to table formatter
 
$delim = $#ARGV >= 1 ? $ARGV[1] : ',';
print STDERR "Split pattern: $delim\n";
 
# first pass
open F, "<$ARGV[0]" or die;
while(<F>)
{
  chomp;
  $i = 0;
  map { $max[$_->[1]] = $_->[0] if $_->[0] > ($max[$_->[1]] || 0) }
    (map {[length $_, $i++]} split($delim));
}
close F;
 
print STDERR 'Field width:   ', join(', ', @max), "\n";
print STDERR join(' ', map {'-' x $_} @max);
 
# second pass
open F, "<$ARGV[0]" or die;
while(<F>)
  {
  chomp;
  $i = 0;
  map { printf("%-$max[$_->[1]]s ", $_->[0]) }
    (map {[$_, $i++]} split($delim));
  print "\n";
}
close F;
```

#### Test for Python

```python
# test python (sample from offlineimap)
 
class ExitNotifyThread(Thread):
    """This class is designed to alert a "monitor" to the fact that a thread has
    exited and to provide for the ability for it to find out why."""
    def run(self):
        global exitthreads, profiledir
        self.threadid = thread.get_ident()
        try:
            if not profiledir:          # normal case
                Thread.run(self)
            else:
                try:
                    import cProfile as profile
                except ImportError:
                    import profile
                prof = profile.Profile()
                try:
                    prof = prof.runctx("Thread.run(self)", globals(), locals())
                except SystemExit:
                    pass
                prof.dump_stats( \
                            profiledir + "/" + str(self.threadid) + "_" + \
                            self.getName() + ".prof")
        except:
            self.setExitCause('EXCEPTION')
            if sys:
                self.setExitException(sys.exc_info()[1])
                tb = traceback.format_exc()
                self.setExitStackTrace(tb)
        else:
            self.setExitCause('NORMAL')
        if not hasattr(self, 'exitmessage'):
            self.setExitMessage(None)
 
        if exitthreads:
            exitthreads.put(self, True)
 
    def setExitCause(self, cause):
        self.exitcause = cause
    def getExitCause(self):
        """Returns the cause of the exit, one of:
        'EXCEPTION' -- the thread aborted because of an exception
        'NORMAL' -- normal termination."""
        return self.exitcause
    def setExitException(self, exc):
        self.exitexception = exc
    def getExitException(self):
        """If getExitCause() is 'EXCEPTION', holds the value from
        sys.exc_info()[1] for this exception."""
        return self.exitexception
    def setExitStackTrace(self, st):
        self.exitstacktrace = st
    def getExitStackTrace(self):
        """If getExitCause() is 'EXCEPTION', returns a string representing
        the stack trace for this exception."""
        return self.exitstacktrace
    def setExitMessage(self, msg):
        """Sets the exit message to be fetched by a subsequent call to
        getExitMessage.  This message may be any object or type except
        None."""
        self.exitmessage = msg
    def getExitMessage(self):
        """For any exit cause, returns the message previously set by
        a call to setExitMessage(), or None if there was no such message
        set."""
        return self.exitmessage
```

#### Test for Bash

```bash
#!/bin/bash
cd $ROOT_DIR
DOT_FILES="lastpass weechat ssh Xauthority"
for dotfile in $DOT_FILES; do conform_link "$DATA_DIR/$dotfile" ".$dotfile"; done
 
# TODO: refactor with suffix variables (or common cron values)
 
case "$PLATFORM" in
    linux)
        #conform_link "$CONF_DIR/shell/zshenv" ".zshenv"
        crontab -l > $ROOT_DIR/tmp/crontab-conflict-arch
        cd $ROOT_DIR/$CONF_DIR/cron
        if [[ "$(diff ~/tmp/crontab-conflict-arch crontab-current-arch)" == ""
            ]];
            then # no difference with current backup
                logger "$LOG_PREFIX: crontab live settings match stored "\
                    "settings; no restore required"
                rm ~/tmp/crontab-conflict-arch
            else # current crontab settings in file do not match live settings
                crontab $ROOT_DIR/$CONF_DIR/cron/crontab-current-arch
                logger "$LOG_PREFIX: crontab stored settings conflict with "\
                    "live settings; stored settings restored. "\
                    "Previous settings recorded in ~/tmp/crontab-conflict-arch."
        fi
    ;;
```
#### Test for Haskell
```haskell
{-# LANGUAGE OverloadedStrings #-}
module Main where
 
--import Prelude hiding (id)
--import Control.Category (id)
import Control.Arrow ((>>>), (***), arr)
import Control.Monad (forM_)
-- import Data.Monoid (mempty, mconcat)
 
-- import System.FilePath
 
import Hakyll
 
 
main :: IO ()
main = hakyll $ do
 
    route   "css/*" $ setExtension "css"
    compile "css/*" $ byExtension (error "Not a (S)CSS file")
        [ (".css",  compressCssCompiler)
        , (".scss", sass)
        ]
 
    route   "js/**" idRoute
    compile "js/**" copyFileCompiler
 
    route   "img/*" idRoute
    compile "img/*" copyFileCompiler
 
    compile "templates/*" templateCompiler
 
    forM_ ["test.md", "index.md"] $ \page -> do
        route   page $ setExtension "html"
        compile page $ pageCompiler
            >>> applyTemplateCompiler "templates/default.html"
            >>> relativizeUrlsCompiler
 
sass :: Compiler Resource String
sass = getResourceString >>> unixFilter "sass" ["-s", "--scss"]
                         >>> arr compressCss
```
#### Test for PHP
```php
<?php
require_once($GLOBALS['g_campsiteDir']. "/$ADMIN_DIR/country/common.php");
require_once($GLOBALS['g_campsiteDir']. "/classes/SimplePager.php");
camp_load_translation_strings("api");
 
$f_country_language_selected = camp_session_get('f_language_selected', '');
$f_country_offset = camp_session_get('f_country_offset', 0);
if (empty($f_country_language_selected)) {
    $f_country_language_selected = null;
}
$ItemsPerPage = 20;
$languages = Language::GetLanguages(null, null, null, array(), array(), true);
$numCountries = Country::GetNumCountries($f_country_language_selected);
 
$pager = new SimplePager($numCountries, $ItemsPerPage, "index.php?");
 
$crumbs = array();
$crumbs[] = array(getGS("Configure"), "");
$crumbs[] = array(getGS("Countries"), "");
echo camp_html_breadcrumbs($crumbs);
 
?>
 
<?php  if ($g_user->hasPermission("ManageCountries")) { ?>
<table BORDER="0" CELLSPACING="0" CELLPADDING="1">
    <tr>
        <td><a href="add.php"><?php putGS("Add new"); ?></a></td>
    </tr>
</table>
```
#### Test for Javascript 
```js
import isTypedArray from 'lodash/isTypedArray';
import reverse from 'lodash/reverse';
import sortBy from 'lodash/sortBy';
import take from 'lodash/take';
import { food101Classes } from './food101';
export function food101topK(classProbabilities, k = 5) {
  const probs = isTypedArray(classProbabilities)
    ? Array.prototype.slice.call(classProbabilities)
    : classProbabilities;
  const sorted = reverse(
    sortBy(
      probs.map((prob, index) => [ prob, index ]),
      probIndex => probIndex[0]
    )
  );
  const topK = take(sorted, k).map(probIndex => {
    const iClass = food101Classes[probIndex[1]];
    return {
      id: probIndex[1],
      name: iClass.replace(/_/, ' '),
      probability: probIndex[0]
    };
  });
  return topK;
};
```
#### Test for HTML
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html><head>
<title>A Tiny Page</title>
<style type="text/css">
<!--
      p { font-size:15pt; color:#000 }
    -->
</style></head><!-- real comment -->
<body bgcolor="#FFFFFF" text="#000000" link="#0000CC">
<script language="javascript" type="text/javascript">
      function changeHeight(h) {
        var tds = document.getElementsByTagName("td");
        for(var i = 0; i < tds.length; i++) {
          tds[i].setAttribute("height", h + "px");
      }}
</script>
<h1>abc</h1>
<h2>def</h2>
<p>Testing page</p>
</body></html>
```
#### Test for CSS
```css
/*
Monokai style - ported by Luigi Maselli - http://grigio.org
*/
.hljs {
  display: block;
  overflow-x: auto;
  padding: 0.5em;
  background: #272822; color: #ddd;
}
.hljs-tag,
.hljs-keyword,
.hljs-selector-tag,
.hljs-literal,
.hljs-strong,
.hljs-name {
  color: #f92672;
}
.hljs-code {
  color: #66d9ef;
}
.hljs-class .hljs-title {
  color: white;
}
```

# Long Paragraphs


Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque vel lacinia neque. Praesent nulla quam, ullamcorper in sollicitudin ac, molestie sed justo. Cras aliquam, sapien id consectetur accumsan, augue magna faucibus ex, ut ultricies turpis tortor vel ante. In at rutrum tellus. Nullam vestibulum metus eu purus malesuada, volutpat mattis leo facilisis. Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.
