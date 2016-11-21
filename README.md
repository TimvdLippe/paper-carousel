[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://beta.webcomponents.org/element/Redbility/paper-carousel)

# Paper-carousel

### Description

Polymer element for displaying a responsive carousel

### Install

First you need bower, [see their site](http://bower.io/) for details

```sh
bower install --save Redbility/paper-carousel
```

### Examples

A simple example of its use:

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-carousel.html">
  </template>
</custom-element-demo>
```
-->
```html
<paper-carousel items="4" responsive="1280:3, 800:2, 460:1" controls="true" dots="true" dotText="false">
	<div class="paper-carousel-demo-indigo" data-text="#1"></div>
	<div class="paper-carousel-demo-pink" data-text="#2"></div>
	<div class="paper-carousel-demo-teal" data-text="#3"></div>
	<div class="paper-carousel-demo-amber" data-text="#4"></div>
	<div class="paper-carousel-demo-blue" data-text="#5"></div>
	<div class="paper-carousel-demo-green" data-text="#6"></div>
</paper-carousel>
```

## Attributes

| Attribute Name | Functionality | Type | Default |
|----------------|-------------|-------------|-------------|
| items | Number of slides shown on each page | Number | 1 |
| responsive | String that contains information about breakpoints | String | null |
| controls | Shows or hides the forward or backward page controls | Boolean | true |
| dots | Shows or hides the navigation dots | Boolean | true |
| dotText | Shows or hides numbers inside dots | Boolean | true |

## Methods

| Method Name | Explanation |
|-------------|-------------|
| getTotalItems() | Gets the number of total items inside carousel |
| getTotalPages() | Gets the number of total pages of carousel |
| getCurrentItem() | Gets the active item |
| goToItem(number) | Moves carousel to the item position |
| goToNextItem() | Moves carousel to the next item |
| goToPrevItem() | Moves carousel to the prev item |
| getCurrentPage() | Gets the active page |
| goToPage(number) | Moves carousel to the page position |
| goToNextPage() | Moves carousel to the next page |
| goToPrevPage() | Moves carousel to the prev page |
| setActiveDot() | Mark a dot element as active |
