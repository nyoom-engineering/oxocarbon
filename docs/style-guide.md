# Style Guide

As the oxocarbon palette is a subset of the IBM Carbon palette, we follow much of IBM's carbon design philosophy as well. Note that *how* much your theme alters UI elements will depend on the application. Certain applications (e.g. terminal emulators, vscode) will be far less theme-able than others (e.g. emacs). In each case, please aim to theme as much as possible

## Colors

Each port *must* contain a dark theme, and optionally may also contain a light theme.

The best place to start are the [base16](https://github.com/nyoom-engineering/base16-oxocarbon) versions of oxocarbon. These are the 16 most notable colors of the carbon palette, and are the colors you will be using most often. Keep in mind that you are not *limited* to these colors, People creating oxocarbon themes are welcome to use colors part of IBM's palette, outside of the base16 defined colors. For example I use `Gray 40` in oxocarbon.nvim's CMP completion menu. However, usage of extra colors should be limited and tasteful

## Anatomy

Oxocarbon’s default themes are derived from the IBM Design Language color palette. The neutral gray family is dominant in the default themes, making use of subtle shifts in value to organize content into distinct zones.

The core blue family serves as the primary action color across all IBM products and experiences. Additional colors are used sparingly and purposefully.

As a general guideline, the two most used colors should be *pink* and *cyan*, with darker blues and subdued pinks/purples used for important but not notable text. You may also use bolding and italicizing as a tool to emphasize important text such as function declartions or comments

## Guidelines

Your most used references are going to be the IBM branding color guidelines (https://www.ibm.com/design/language/color/) and the carbon design systems color guidelines (https://carbondesignsystem.com/guidelines/color/overview/). The most notable guidelines to keep in mind are

Backgrounds/Foregrounds:

- Background colors follow a layering model. The darkest black (base00) should always be the background color, and any UI elements should always use a lighter tone of black (e.g. base01 or base02).
- Foreground colors follow a similar model, except that instead of getting lighter and lighter, you may alternate between the lightest color in the theme (base06) and the second/third lighest (base05, base04)

<img width="823" alt="image" src="https://user-images.githubusercontent.com/71196912/206875348-b3f24d9a-81c1-49f9-bbb4-f4e3f65dbdec.png">

- For readability reasons, do not apply components that are darker than the background, except in special cases

<img width="863" alt="image" src="https://user-images.githubusercontent.com/71196912/206875206-b59a413d-82cb-4fc1-9091-7d90f0c4cddd.png">

- Its important to maintain proper contrast at all times. Based off of the <https://www.w3.org/TR/WCAG21/>, small text is any size below 24px and requires a 4.5:1 contrast ratio. Large text is anything above 24px and requires a 3:1 contrast ratio. Graphical elements, such as data visualizations, also require a 3:1 contrast ratio. The IBM palette is comprised of twelve color grades—Black, White and ten values for each hue. The following table indicates the minimum number of steps required to achieve commonly used contrast ratios between any two colors.

<img width="548" alt="image" src="https://user-images.githubusercontent.com/71196912/206875056-77d3aafd-8323-4e08-90da-2c725e42a8b1.png">

<img width="963" alt="image" src="https://user-images.githubusercontent.com/71196912/206875119-73543502-0094-495e-a7b6-0584b7dae2bf.png">


Code/Colors
- Respect the 4/3/2 color sets that IBM has created. 
<img width="590" alt="image" src="https://user-images.githubusercontent.com/71196912/206875287-143e1806-6615-4cee-868e-db20e61df6b0.png">
<img width="588" alt="image" src="https://user-images.githubusercontent.com/71196912/206875293-0e28f70a-4cef-4170-82b1-52b4bda6d5fc.png">
<img width="588" alt="image" src="https://user-images.githubusercontent.com/71196912/206875298-429a467c-b04d-47f5-9574-2eeacca9ab83.png">

- Avoid mixing greens with reds, magentas or purples.
- Avoid mixing teals with reds or magentas.

<img width="652" alt="image" src="https://user-images.githubusercontent.com/71196912/206875306-332faebb-d0b8-48e7-99e7-8e55b04987fc.png">

- Avoid using gradients
