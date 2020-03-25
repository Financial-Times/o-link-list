# o-link-list [![Build Status](https://circleci.com/gh/Financial-Times/o-link-list.png?style=shield&circle-token=34ef68c62eb057caad5ece702c6078b2708d4647)](https://circleci.com/gh/Financial-Times/o-link-list) [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](#licence)

_Deprecated, please speak to the Origami team if you would like to use a component like o-link-list._

Styles for lists of links typically used in navigation elements and asides.

- [Usage](#usage)
	- [Markup](#markup)
	- [Sass](#sass)
- [Migration guide](#migration-guide)
- [Contact](#contact)
- [Licence](#licence)


## Usage

### Markup

The suggested markup used for this module depends on the context within the page.

#### Markup for navigational elements

If the list is a list of links with a navigational purpose then the following markup should be used.
We suggest avoiding `<li>` in combination with a `<nav>` as it increases the amount of reading a screen reader will do without adding value to the user.

```
<nav class="o-link-list" >
  <a class="o-link-list__item" href='#'>item 1</a>
  <a class="o-link-list__item" href='#'>item 2</a>
  <a class="o-link-list__item" href='#'>item 3</a>
  <a class="o-link-list__item" href='#'>item 4</a>
  <a class="o-link-list__item" href='#'>item 5</a>
  <a class="o-link-list__item" href='#'>item 6</a>
  <a class="o-link-list__item" href='#'>item 7</a>
</nav>
```

In the event that this list is being used in an `<aside>`, `<li>` elements should be used along with an optional title.

```
<aside class="o-link-list">
  <div class="o-link-list__aside-title">Topics mentioned in this article</div>
  <ul class="o-link-list__item-container" >
    <li><a class="o-link-list__item" href="#">item 1</a></li>
    <li><a class="o-link-list__item" href="#">item 2</a></li>
    <li><a class="o-link-list__item" href="#">item 3</a></li>
    <li><a class="o-link-list__item" href="#">item 4</a></li>
    <li><a class="o-link-list__item" href="#">item 5</a></li>
    <li><a class="o-link-list__item" href="#">item 6</a></li>
    <li><a class="o-link-list__item" href="#">item 7</a></li>
  </ul>
</aside>
```

### Sass

## Silent mode

When you're not consuming this module via the build service, by default this module is set to 'silent' - meaning its Sass will not output any CSS classes, only Sass mixins.

When `$o-link-list-is-silent: false;`, the module outputs a set of classes that are also documented in each section

## Migration guide

### Updating from v1 to v2

V1 -> V2 introduces the new major of o-colors. Updating to this new version will mean updating any other components that you have which are using `o-colors`. There are no other breaking changes in this release.

---

## Contact

If you have any questions or comments about this component, or need help using it, please either [raise an issue](https://github.com/Financial-Times/o-link-list/issues), visit [#ft-origami](https://financialtimes.slack.com/messages/ft-origami/) or email [Origami Support](mailto:origami-support@ft.com).

----

## Licence

This software is published by the Financial Times under the [MIT licence](http://opensource.org/licenses/MIT).

