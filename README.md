# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U).


## Overview

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

I am on my way to complete as many Level 1 Newbie challenges as I can before I advance to the next level.

### What I learned

The main difficulty in this challenge was to get another image to hover over the existing one. While I have experimented with hovering over links and text, I did not know how to make another image appear. I spent some time watching tutorials and reading posts from W3 Schools, and I was able to figure it out. In simple terms, it is messing around with divs and placing one on top of the other!

I had three divs in the end:
1 - equilibrium
2 - overlay
3 - view

This was what I ended up with:

```css

.equilibrium-image {
  position: relative;
  width: 245px;
  height: 245px;
  border-radius: 10px;
  left: 15px;
  right: 15px;
  top: 15px;
}

.overlay {
  position: absolute;
  width: 245px;
  height: 245px;
  top: 15px;
  left: 15px;
  border-radius: 10px;
  opacity: 0;
  transition: opacity 0.4s ease-in-out;
  background: hsl(178, 100%, 50%);
}

.view {
  position: relative;
  width: 50px;
  height: 50;
  top: 100px;
  left: 100px;
}

.equilibrium:hover .overlay {
  opacity: 0.5;
  cursor: pointer;
}
```
Equilibrium-image was the image's class. There's more context in the other files.

### Continued development

In the future, I want to explore the hover selector more. While looking up tutorials, I all sorts of animations using the hover selector, I want to try those for myself.


## Author

Frontend Mentor - [@sanikasurose](https://www.frontendmentor.io/profile/sanikasurose)
