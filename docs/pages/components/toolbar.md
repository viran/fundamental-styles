---
title: Toolbar
id: toolbar
keywords: toolbar
sidebar: left-navigation-sidebar
toc: false
permalink: components/toolbar.html
folder: components
summary:
---

The toolbar enables the user to change the UI or trigger an action. For example, the toolbar allows the user to change views, manipulate data or objects, navigate to another page, perform generic actions, and so on.
{: .docs-intro}

## Toolbar types

### Solid

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid">
    <span>Title</span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__separator"></span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### Auto

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--clear fd-toolbar--auto">
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__separator"></span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### Transparent

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--clear fd-toolbar--transparent">
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__separator"></span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### Info

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    3 item selected
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### Title

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--solid fd-toolbar--title fd-toolbar-active">
    <span>Title</span>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"></span>
    <button>opt1</button>
    <button>opt2</button>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

## Spacer

Its role is to fill remaining space either automatically or manually and place item regarding to it

### Auto

Takes remaining width and fill it

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--info fd-toolbar--active">
    <span>text</span>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"></span>
    <span>text</span>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### Fixed

Developer has to set width for spacer

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__spacer" style="width:150px;"></span>
    <span>text</span>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

## Separator

Its role is to visually separate items from each other
{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>
  
  <br>
  
  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}

## Directory

### LTR

Its role is to visually separate items from each other
{% capture toolbar %}

<div dir="ltr">
  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>
  
  <br>
  
  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>

  <br>

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__spacer" style="width:150px;"></span>
    <span>text</span>
  </div>

</div>

{% endcapture %}
{% include display-component.html component=toolbar %}

### RTL

Its role is to visually separate items from each other
{% capture toolbar %}

<div dir="rtl">
  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>
  
  <br>
  
  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid">
    <span>text</span>
    <span class="fd-toolbar__separator"></span>
    <span>text</span>
  </div>
  
  <br>

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--info">
    <span>text</span>
    <span class="fd-toolbar__spacer" style="width:150px;"></span>
    <span>text</span>
  </div>

</div>
{% endcapture %}
{% include display-component.html component=toolbar %}
