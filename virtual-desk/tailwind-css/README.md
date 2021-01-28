# Tailwindcss
* [What I understood?](#what-I-understood)
* [Impressions](#impressions)
* [Resources](#resources)

# What did I understand?
Tailwindcss is a way of writing CSS without CSS Syntax.  In normal circumstances, If you want to have a button that has a background color on the index page, you have to follow these steps;

#### Step 1: Add an element
```html
<!-- index.html -->
<button>Button</button>
```
#### Step 2: Set styles for the button
```css
/* index.css */
button {
	background-color: red;
}
```
Tailwind provides an extended styling property memory as a large number of classes on your project and all of this possible with `3.74MB`. At the top, I created two files as `index.css` and `index.html`. 

But the same work, can be possible without a css file while feeding by Tailwind's utility classes. 

## How does it work?
You don't have to create a css file to do styling on your html with Tailwindcss 
```html
<!-- I just use bg-red-500 class instead of having custom styles -->
<button class="bg-red-500">Button</button>
```
I was like, "They can't do everything with classes." until I started to use it. I realize that they have a large number of detailed utilities to able to control every single property of CSS. Let's deep dig into an example of a utility;

>  `bg-red-500` is a utility class name that used on my last example at the top. 

They have detailed documentation for each utility. In my example, background color utility has two different props as `color` and `alpha`. Here is a skeleton of this utility;

`bg-{color}-{alpha}`: In my example, I used as `bg-red-500`.

## Customizing
Also, you can customize your tailwind template with tailwind.config.js. If you want to add your style guide's color palette instead of the default, you only need to update the config file then you ready to go. Here is an example;
```js
// tailwind.config.js
module.exports = {
  theme: {
    backgroundColor: theme => ({
      primary: {
        100: '#3490dc',
        500: '#ffed4a',
        600: '#e3342f',
      },
    }),
  },
}
```
```html
<!-- index.html -->
<button class="bg-primary-100">Button</button>
```
After having this config file in your project folder. You will able to use `bg-primary-500`. 

So, In short; The documentation says:

> A utility-first CSS framework packed with classes like flex, pt-4, text-center and rotate-90 that can be composed to build any design, directly in your markup. (1)

# Impressions
I realized that Tailwindcss is what I had wished for [in 2017](https://github.com/volcanioo/Muesnet-CSS-Framework#grid-system-in-percent "in 2017"). After watching a short tutorial by [Dan Vega](https://www.youtube.com/watch?v=xP_uJj8L_1Q "Dan Vega"), I only opened the [documentation](https://tailwindcss.com/docs/ "documentation") and spent a little bit of time on the utility section. So, That was a delightful work case for me.  

Happy to see something like this in real! If you want to discuss something, here is this file's [discussion.](https://github.com/volcanioo/volcanioo/discussions/2)

# Resources

1. https://tailwindcss.com/
2. https://www.youtube.com/watch?v=xP_uJj8L_1Q
3. https://tailwindcss.com/docs/background-color#customizing

