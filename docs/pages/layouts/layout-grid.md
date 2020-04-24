---
title: Layout Grid
id: layout_grid
keywords: layout_grid
sidebar: left-navigation-sidebar
toc: false
permalink: layouts/layout-grid.html
folder: layouts
summary:
---

{: .docs-intro}

## Layout Grid

Use the `fd-col` to create a column of a certain width. The default value will create a column the full width of the parent at size small and above unless specified another size .

## Default Layout Grid (12 columns)
{% capture default %}
<div class ="fd-container__outer">
    <div class="fd-container">
        <div class="fd-row">
            <div class="fd-col">
                <div style="background-color: #8a8a8a;text-align:center;width:100%;">
                Default 12 column
                </div>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=default %}

<br/>


## Layout Grid with sizing (6 columns for all)
To define the size of that column use the `fd-col--x` modifier, where x can go from 1-12, or 1-16 with the extra large size modifier.
{% capture size %}
<div class ="fd-container__outer">
    <div class="fd-container">
        <div class="fd-row">
            <div class="fd-col fd-col--6">
                <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                6 col at each size
                </div>
            </div>
            <div class="fd-col fd-col--6">
                <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                    6 col at each size
                </div>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=size %}

<br/>

## Layout Grid for form
To define the size of that column use the `fd-col--x` modifier, where x can go from 1-12, or 1-16 with the extra large size modifier.
{% capture size %}
<div class ="fd-container__outer">
    <div class="fd-container">
        <div class="fd-row">
            <div class="fd-col fd-col--4">
                <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                4 col
                </div>
            </div>
            <div class="fd-col fd-col--7">
                <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                    7 col
                </div>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=size %}

<br/>

##  Layout Grid with sizing and responsiveness
Add the `fd-col--col-x--size` to define that column size only for a certain screen size and above
{% capture breakpoints %}
<div class ="fd-container__outer">
    <div class="fd-container">
        <div class="fd-row">
            <div class="fd-col fd-col--6--l">
                <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                    12 col under large, 6 at large
                </div>
            </div>
            <div class="fd-col fd-col--6--l">
                <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                    12 col under large, 6 at large
                </div>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=breakpoints %}
<br/>


##  Layout Grid with nesting
Add an extra `fd-row` class when using more than one row or nesting.
{% capture layout-grid-multi-level %}
<div class ="fd-container__outer">
    <div class="fd-container">
        <div class="fd-row">
            <div class="fd-col fd-col--6">
                <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                    6 col
                </div>
                <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                    6 col
                </div>
            </div>
            <div class="fd-col fd-col--6">
                <div class="fd-row">
                    <div class="fd-col fd-col--4">
                        <div style="background-color: #8a8a8a;text-align:center;width:100%;"> 
                            4 col outer
                        </div> 
                    </div>
                    <div class="fd-col fd-col--8">
                        <div class="fd-row">
                            <div class="fd-col fd-col--12">
                                <div style="background-color: #4a4a4a;text-align:center;width:100%;">
                                    12 out of 8 col
                                </div>
                            </div>      
                            <div class="fd-col fd-col--12">
                                <div class="fd-row">
                                    <div class="fd-col fd-col--6">
                                        <div style="background-color: #666666;text-align:center;width:100%;">
                                        6 out of 12 out of 8 col
                                        </div>
                                    </div>
                                    <div class="fd-col fd-col--6">
                                        <div style="background-color: #2b2b2b;text-align:center;width:100%;color:white;">
                                        6 out of 12 out of 8 col 
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=layout-grid-multi-level %}

<br/>

##  Layout Grid with offset
To add an offset ot the left of the column use the `--offset-x` modifier. X will be the size of your choice. If the column after the offset col no longer fits in parent container it will switch to the next page
{% capture layout-grid-multi-level %}
<div class="fd-container">
    <div class="fd-row">
        <div class="fd-col fd-col--6">
            <div style="background-color: #2b2b2b;text-align:center;width:100%;color:white;">
                6 col
            </div>
        </div>
        <div class="fd-col fd-col--4 fd-col--offset-1">
            <div style="background-color: #8a8a8a;text-align:center;width:100%;"> 
                4 col with offset of 1
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=layout-grid-multi-level %}

<br/>


<br/>

##  Layout Grid with multiple rows
To use multiple rows, make `fd-row` siblings with each other. This will cause a line break for the new row.
{% capture layout-grid-multi-level %}
<div class="fd-container">
    <div class="fd-row">
        <div class="fd-col fd-col--12">
            <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                12 col row 1
            </div>
        </div>
        <div class="fd-col fd-col--4">
            <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                4 col row 1
            </div>
        </div>
    </div>
    <div class="fd-row">
        <div class="fd-col fd-col--6">
            <div style="background-color: #8a8a8a;text-align:center;width:100%;">>
                6 col row 2
            </div>
        </div>
        <div class="fd-col fd-col--6">
            <div style="background-color: #4a4a4a;text-align:center;width:100%;">>
                6 col row 2
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=layout-grid-multi-level %}

<br/>

##  Layout Grid with no gap
To remove gutters between columns apply the `fd-container--no-gap` modifier for the container and the `fd-col--no-gap` modifier with the column.
{% capture layout-grid-multi-level %}
<div class="fd-container fd-container--no-gap">
    <div class="fd-row">
        <div class="fd-col fd-col--6 fd-col--no-gap">
            <div style="background-color: #dbdbdb;text-align:center;width:100%;">
                6 col no gap
            </div>
        </div>
        <div class="fd-col fd-col--6 fd-col--no-gap">
            <div style="background-color: #bdbdbd;text-align:center;width:100%;">
                6 col no gap
            </div>
        </div>
    </div>
</div>
{% endcapture %}
{% include display-component.html component=layout-grid-multi-level %}

<br/>