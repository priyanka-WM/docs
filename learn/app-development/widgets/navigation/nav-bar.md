---
title: "Nav Bar"
id: ""
---

![](/learn/assets/laptop.png)  **NOTE**: Nav Bar is available only for web responsive apps.

**Nav Bar Widget** can be used to create responsive navigation header for your website or application. These responsive navbars are initially collapsed on devices having small viewports like cell-phones but expand when user click the toggle button. However, it will be horizontal as normal on the medium and large devices like laptop or desktop.

You can also create different variations of the navbar such as navbars with drop-down menus and search boxes as well as fixed positioned navbar with much less effort.

<iframe width="100%" height="100" style="background-color: snow;" allowtransparency="true" src="https://apps.wavemakeronline.com/documentation_snippets/#/Navbar">Navbar</iframe>

**WaveMaker Nav Bar** widget is used in the implementation of the default _topnav_ when the [page layout](/learn/app-development/ui-design/page-concepts/page-layouts/) is chosen to include the same. Following features are available:

1. _Title_ and _image _for the navbar can be specified
2. Two _nav widgets_ are provided and each can be customized to include Anchor, Menu, Popover, Button. Each of these nav widgets is aligned to the left and right of the Nav Bar. [Click here for nav widget usage](/learn/app-development/widgets/navigation/nav/).

# Properties

| Property | Description |
| --- | --- |
| Title | Set the title of the Navbar. This name is used for the first (home) link of the navbar. |
| Name | The name is a unique identifier for Navbar. |
| Home Link | This property can be used to specify the URL for the home link. By default, this is set to the Home page set in the Project Configuration dialog. |
| **Layout** |
| Height | The height of your widget can be specified in px or % (i.e 50px, 75%). |
| Image Source | This bindable property specifies the source for the brand image. The source can be either a file or a URL:
- File: enter the directory and filename for the image to display (supported file types include .jpg, .gif and .png). By default, WaveMaker looks for images in the src/main/webapp directory of the project.
- URL: enter a URL to any internet-accessible image. To display the file, foo.jpg, in the project directory src/main/webapp/resources/images/imagelists/, enter the following into the source property:resources/images/imagelists/foo.jpg or simply foo.jpg

 |
| **Behavior** |
| Show | Showing determines whether or not a component is visible. It is a bindable property. |
| Load on Demand (visible only when show property is bound to a variable) | When this property is set and show property is bound, the initialization of the widget will be deferred till the widget becomes visible. This behavior improves the load time. Use this feature with caution, as it has a downside (as we will not be able to interact with the widget through script until the widget is initialized). When show property is not bound the widget will be initialized immediately. |
| Menu icon | This property sets the icon for the menu button that will appear in the mobile layout ONLY. |

[6\. Navigation Widgets](/learn/app-development/widgets/widget-library/#nav-widgets)

- [6.1 Breadcrumb](/learn/app-development/widgets/navigation/breadcrumb/)
- [6.2 Dropdown Menu](/learn/app-development/widgets/navigation/dropdown-menu/)
- [6.3 Nav](/learn/app-development/widgets/navigation/nav/)
- [6.4 Nav Bar](/learn/app-development/widgets/navigation/nav-bar/)
    - [i. Properties](#properties)
- [6.5 Popover](/learn/app-development/widgets/navigation/popover/)
