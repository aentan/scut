# Scut

**&mdash; a collection of Sass (SCSS) mixins and placeholders for common styling patterns.**

You can think of the word Scut as an acronym for ***SC***SS ***Ut***itilies.

<small>(Or you can think of the word in other ways: Scut will do your *scut work*; let Scut be your *scut monkey*. (Be careful how you use this word in polite company. To learn its many and colorful connotations, [have a look at Wiktionary](http://en.wiktionary.org/wiki/scut).))</small>

**BE AWARE:** Scut is in early stages, under active development, *unstable* &mdash; still in [SemVer](http://semver.org/) v0. **Scut is wide, wide open to contributions**, and I will be building on it myself. New features will be added and old features might change. So: **if some part of Scut that you had been using suddenly doesn't work, please check this documentation to see what changed.**

<a href="https://github.com/davidtheclark/scut/" class="intro-btn">Visit the Github repository</a>

<a href="http://codepen.io/davidtheclark/pen/yCadJ" target="_blank" class="intro-btn">Experiment with Scut on Codepen</a>

### Why use Scut?

#### Avoid repetition

Scut's primary goal is to save people like you and me from repeating the same few lines of styling code, over and over again, to achieve the same effect in different places.

#### Organize your rules

An oft-unsung quality of mixins and placeholders is that they organize your code, *grouping rules according to the effects they combine to achieve*. Even when a mixin applies only a couple of rules (like [`scut-hanging-indent`](#hanging_indent)), it serves this end.

#### Save some Google searching

As we would all like to spend a smaller percentage of our lives sitting at red lights, we also hope to spend less life flicking through search results.

#### Implement best practices

Some of Scut's utilities, such as [`hd-breakpoint`](#hd_breakpoint) and [`font-face`](#font-face), are all about implementing "best practices" &mdash; without looking them up every time you need them.

*If somebody figures out a better way to do it, with better browser support, fewer extra `<div>`s, whatever, Scut should be updated accordingly. **So contribute your fabulous ideas and discoveries!***

### What makes Scut unique?

#### Flexible abstractions of common patterns &mdash; nothing more

Scut doesn't require additional setup and processing, doesn't apply any default sizes, spacing, colors, etc. It strives to be as simple, flexible, and un-opinionated as possible, offering abstract patterns that you can work into your own designs without having to override anything or set up site-wide parameters.

#### No vendor prefixes

Some other pre-processor libraries do little more than vendor prefixing. Scut doesn't bother with that: we're looking for other things to do.

Most of Scut's utilities do not use properties that require vendor prefixes. But **if a utility *does* require vendor prefixing, you should be warned in the documentation below. In such cases *and all other cases* Scut suggests that you install and run [Autoprefixer](https://github.com/ai/autoprefixer) as part of the compilation process.** (I rely on [Grunt](http://gruntjs.com/) to make this happen, with the [grunt-autoprefixer plugin](https://github.com/nDmitry/grunt-autoprefixer). Easy as can be.)

#### @extend placeholders

All mixins that require no arguments &mdash; either because they *have* no arguments or because all their arguments have default values &mdash; are paired with [placeholder selectors](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html#placeholders), which are good things to use, when you can.

#### `scut-` prefix

To avoid confusions and collisions, all Scut utilities &mdash; mixins, placeholders, and functions &mdash; are prefixed with `scut-`.

## <a href="#installation" id="installation" class="inner-anchor">Installation</a>

1. Get the files. You have the following options:<div class="install-list">
  - **Use [Bower](http://bower.io/) (*recommended*): <pre class="language-bash"><code>bower install scut --save-dev</code></pre>** This will get you the latest release, without superfluous files, and save it as a devDependency.
   - Download [the latest release from Github](https://github.com/davidtheclark/scut/releases).</div>

2. Then, from your own Sass/SCSS files, import `_scut.scss`. Like this: <pre class="language-scss"><code>@import "path/to/scut";</code></pre>

`_scut.scss` is a concatenation of all the files in `src/`. To inspect the code you're using, you could look in either place.

Make sure you import Scut *above* any other stylesheets that will rely on it.

## <a href="#usage" id="usage" class="inner-anchor">Usage</a>

Having imported `_scut.scss`, use the mixins and placeholders described below in the manner described below.

If you have any questions about how to use Sass/SCSS, refer to [the thorough Sass documentation](http://sass-lang.com/docs/yardoc/file.SASS_REFERENCE.html).

If the Scut documentation below is inadequate or upsetting, please [file an issue](https://github.com/davidtheclark/scut/issues) or [contact me](https://github.com/davidtheclark).

If you have been using Scut already, then you get a new version and something breaks, please check the documentation again to see if the utility has changed slightly. *Scut is still in the unstable stages of v0, so these things might happen.*

And again, *you should probably install and use [Autoprefixer](https://github.com/ai/autoprefixer)* if you want vendor prefixes (which you do). Scut won't take care of those.

### Browser Support

For most of Scut's utilities, browser support should include any modern browser and IE8+.

If a specific utility *does* have broader compatibility issues, they should be noted in the documentation below.

## <a href="#contributing" id="contributing" class="inner-anchor">Contributing</a>

Please do!

Just [visit the repository on Github](https://github.com/davidtheclark/scut) and file issues and pull requests according to the usual Github methods. A little contribution guide is included in the README there.

If you have any questions, please [file an issue](https://github.com/davidtheclark/scut/issues) or [contact me](https://github.com/davidtheclark).