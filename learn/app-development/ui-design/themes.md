---
title: "Themes"
id: "themes"
---
---

**Themes** are style elements which work at the widget or UI component level. Themes help you provide a consistent look and feel to your application. 

## Styling Elements
Theme mainly contains the following styling for all the elements on the page:

1. **Color**: Background, text color, border color, hover/active/focus colors, and more.
2. **Properties**: For text like text-align, text-decoration, font-size, font-weight, and more.
3. **Layout**: Includes margin, padding, border-radius, and more.

## Theme Concepts

In this document the following concepts are explained:

- [Applying themes](#applying-theme)
- [Importing custom themes](#importing-theme)
- [Creating themes](#create-theme) for WaveMaker [web apps](#create-theme-web), [using Bootswatch](#create-theme-bootswatch), and for [mobile apps](#create-theme-mobile)
- [Building](#build-theme)
- [Testing](#test-theme) or changing theme temporarily
- [Publishing](#publish-theme)
- [Theme package structure](#theme-packaging)

## Applying Theme

1. To **change the theme** for a page, simply click on the **Themes** option from the _Workspace Toolbar:_

[![](/learn/assets/theme_change.png)](/learn/assets/theme_change.png)

2. This will open a Theme dialog with a list of available themes to choose from.

[![](/learn/assets/Themes.png)](/learn/assets/Themes.png) 

:::note
WaveMaker provides a few default themes that can be applied to your apps. From time to time, these Themes might undergo changes and you might be asked to update the theme when you open the project.  
:::

:::warning
Remember that the updates will re-write any changes you made directly to the CSS styles of the corresponding theme.
:::

## Importing Theme

You can use your own theme by importing it into your app. For more information, see [Creating Theme](#creating-theme).

:::note
For Enterprise version, the custom themes will be available once they are published to the EDN and approved by the EDN Admin, without needing to import.
:::

From the above Themes dialog, choose the **Import Theme** button for a pop-up window which will allow you to select a WaveMaker theme zip file. Once imported, the Theme will appear in the _Theme dialog_. To apply the theme, select the imported theme and **Re-Apply**.

## Hybrid Mobile

In a hybrid app mobile theme, there can be different flavors for android and ios systems. Hence, in a theme bundle, there are different folders for android and ios.

Following is the package structure:

<table><tbody><tr><td>Sub-Folder</td><td>Name</td><td>Description</td><td></td></tr><tr><td>none</td><td>.wmproject.properties</td><td>Containing essential properties required to identify the theme which includes the <em>name</em> of the theme, <em>version</em> of the theme, a short meaningful <em>description</em> of the theme, the <em>type</em> should be THEME (DO NOT CHANGE THIS), and the name of the <em>author</em> for the theme.</td><td>Required</td></tr><tr><td>none</td><td>theme.png</td><td>Theme icon.</td><td>Required</td></tr><tr><td>Android</td><td>Fonts</td><td>Folder containing web-based fonts used in the app.</td><td>Required</td></tr><tr><td></td><td>style.css</td><td>Containing styles related to the theme.</td><td>Required</td></tr><tr><td></td><td>variables.less</td><td>LESS variables to define colors, sizes and more.</td><td>Required</td></tr><tr><td>ios</td><td>Fonts</td><td>Folder containing web-based fonts used in the app.</td><td>Required</td></tr><tr><td></td><td>style.css</td><td>Containing styles related to the theme.</td><td>Required</td></tr><tr><td></td><td>variables.less</td><td>Less variables to define colors, sizes and more.</td><td>Required</td></tr></tbody></table>


