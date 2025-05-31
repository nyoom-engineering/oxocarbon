# Style Guide

As the oxocarbon palette is inspired by the original carbon palette, we follow much of their design philosophy as well. Note that *how* much your theme alters UI elements will depend on the application. Certain applications (e.g. terminal emulators, vscode) will be far less theme-able than others (e.g. emacs). In each case, please aim to theme as much as possible

## Colors

The best place to start are the [base16](https://github.com/nyoom-engineering/base16-oxocarbon) versions of oxocarbon. These are the 16 most notable colors of the carbon palette, and are the colors you will be using most often. Keep in mind that you are not *limited* to these colors, People creating oxocarbon themes are welcome to use colors part of the original carbon palette, outside of the base16 defined colors. For example, we use `Gray 40` in oxocarbon.nvim's completion completion menu. However, usage of extra colors should be limited and tasteful

## Guidelines

You should be referencing the original carbon guidelines where possible (https://carbondesignsystem.com/guidelines/color/overview/). The most notable guidelines to keep in mind are.

Backgrounds/Foregrounds:

- Background colors follow a layering model. The darkest black (base00) should always be the background color, and any UI elements should always use a lighter tone of black (e.g. base01 or base02).
- Foreground colors follow a similar model, except that instead of getting lighter and lighter, you may alternate between the lightest color in the theme (base06) and the second/third lighest (base05, base04)

<img width="823" alt="image" src="https://user-images.githubusercontent.com/71196912/206875348-b3f24d9a-81c1-49f9-bbb4-f4e3f65dbdec.png">

- For readability reasons, do not apply components that are darker than the background, except in special cases

<img width="863" alt="image" src="https://user-images.githubusercontent.com/71196912/206875206-b59a413d-82cb-4fc1-9091-7d90f0c4cddd.png">

- Its important to maintain proper contrast at all times. Based off of the <https://www.w3.org/TR/WCAG21/>, small text is any size below 24px and requires a 4.5:1 contrast ratio. Large text is anything above 24px and requires a 3:1 contrast ratio. Graphical elements, such as data visualizations, also require a 3:1 contrast ratio. The carbon palette is comprised of twelve color grades—Black, White and ten values for each hue. The following table indicates the minimum number of steps required to achieve commonly used contrast ratios between any two colors.

<img width="548" alt="image" src="https://user-images.githubusercontent.com/71196912/206875056-77d3aafd-8323-4e08-90da-2c725e42a8b1.png">

<img width="963" alt="image" src="https://user-images.githubusercontent.com/71196912/206875119-73543502-0094-495e-a7b6-0584b7dae2bf.png">


Code/Colors
- Respect the 4/3/2 color sets. 
<img width="590" alt="image" src="https://user-images.githubusercontent.com/71196912/206875287-143e1806-6615-4cee-868e-db20e61df6b0.png">
<img width="588" alt="image" src="https://user-images.githubusercontent.com/71196912/206875293-0e28f70a-4cef-4170-82b1-52b4bda6d5fc.png">
<img width="588" alt="image" src="https://user-images.githubusercontent.com/71196912/206875298-429a467c-b04d-47f5-9574-2eeacca9ab83.png">

- Avoid mixing greens with reds, magentas or purples.
- Avoid mixing teals with reds or magentas.

<img width="652" alt="image" src="https://user-images.githubusercontent.com/71196912/206875306-332faebb-d0b8-48e7-99e7-8e55b04987fc.png">

- Avoid using gradients

# Branding

Branding for the Oxocarbon project is a derivitive of that instilled across the Nyoom Engineering organization. The template should handle most of it for you, but in the case you would like to do it manually, you are welcome to use the standard logos:

<img src="./out/icon-3840x3840-shadow.png" width="345">
<img src="./out/logo-3840x1280-shadow.png" width="345">

Or generate [your own](https://github.com/nyoom-engineering/nyoom-engineering):

<img src="https://github.com/nyoom-engineering/nyoom-engineering/blob/main/out/logo-custom-3840x1330-shadow.png?raw=true" width="345">

Or display the standard palette:

<img src="https://github.com/nyoom-engineering/nyoom-engineering/blob/main/out/palette-3840x4663-shadow.png?raw=true" width="345">

And for websites and the like, there is also a "Made With Oxocarbon" tag you can use: 

<img src="https://github.com/nyoom-engineering/nyoom-engineering/blob/main/out/made-with-3840x1330-shadow.png?raw=true" width="345">

For official ports, a `1280x` resolution banner image with the name of your project should be generated for GitHub's "Social Preview"