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
    <h4 style="margin-bottom:0px;">Title</h4>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"></span>
    <button class="fd-button fd-button--compact fd-button--transparent">opt1</button>
    <button class="fd-button fd-button--compact fd-button--transparent">opt2</button>
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
    <span class="fd-toolbar__spacer fd-toolbar__spacer--fixed" style="width:150px;"></span>
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

## Size

Default size is compact but this can be changed using `fd-toolbar--cozy` modifier

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid fd-toolbar--cozy">
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

## Size

Default size is compact but this can be changed using `fd-toolbar--cozy` modifier

{% capture toolbar %}

  <div class="fd-toolbar fd-toolbar--active fd-toolbar--solid fd-toolbar--cozy">
    <span>Title</span>
    <span class="fd-toolbar__spacer fd-toolbar__spacer--auto"> </span>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <button class="fd-button fd-button--compact fd-button--transparent">Button</button>
    <div class="fd-popover">
      <div class="fd-popover__control">
        <button class="fd-button fd-button--transparent fd-button--compact sap-icon--overflow"
                    aria-controls="wgxzK859" aria-haspopup="true" aria-expanded="false" aria-label="More"></button>
      </div>
      <div class="fd-popover__body fd-popover__body--right" aria-hidden="true" id="wgxzK859">
        <nav class="fd-menu" id="">
          <ul class="fd-menu__list fd-menu__list--no-shadow">
              <li class="fd-menu__item">
                  <a class="fd-menu__link" href="#">
                      <span class="fd-menu__title">Edit</span>
                  </a>
              </li>
              <li class="fd-menu__item">
                  <a class="fd-menu__link" href="#">
                      <span class="fd-menu__title">Delete</span>
                  </a>
              </li>
              <li class="fd-menu__item">
                  <a class="fd-menu__link" href="#">
                      <span class="fd-menu__title">Assign</span>
                  </a>
              </li>
              <li class="fd-menu__item">
                  <a class="fd-menu__link" href="#">
                      <span class="fd-menu__title">Expire</span>
                  </a>
              </li>
              <li class="fd-menu__item">
                  <a class="fd-menu__link" href="#">
                      <span class="fd-menu__title">Archive</span>
                  </a>
              </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>

{% endcapture %}
{% include display-component.html component=toolbar %}
