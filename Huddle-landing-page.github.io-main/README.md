# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![Desktop solution](images/Desktop.PNG)
![Mobile solution](images/Mobile.PNG)

### Links

- Solution URL: [GitHub solution](https://github.com/TrnLinh/Huddle-landing-page.github.io.git)
- Live Site URL: [Website solution](https://trnlinh.github.io/Huddle-landing-page.github.io/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid

### What I learned

Better way to organise html

```html
<section>
  <div class="logo-container">
    <img src="images/logo.svg" alt="logo" class="logo" />
  </div>
  <div class="container">
    <div class="grid-container">
      <div class="left">
        <div class="img-container">
          <img src="images/illustration-mockups.svg" alt="" class="img" />
        </div>
      </div>
      <div class="right">
        <p class="title">
          Build The Community <br />
          Your Fans Will Love
        </p>
        <p class="content">
          Huddle re-imagines the way we build communities. You have <br />
          a voice, but so does your audience. Create connections with <br />
          your users as you engage in genuine discussion.
        </p>
        <div class="link">
          <a href="#" class="Regist">Register</a>
        </div>
      </div>
    </div>
    <div class="icon-container">
      <a
        href="https://www.facebook.com/profile.php?id=100028496047515"
        class="icon"
        target="_blank"
      >
        <i class="fab fa-facebook-square"></i>
      </a>
      <a
        href="https://www.instagram.com/_trnlinh_/?hl=en"
        class="icon"
        target="_blank"
      >
        <i class="fab fa-instagram"></i>
      </a>
      <a href="https://github.com/TrnLinh" class="icon" target="_blank">
        <i class="fab fa-github"></i>
      </a>
    </div>
  </div>
</section>
```

```css
section {
  display: grid;
  min-height: 100vh;
}
.logo {
  margin-top: 20px;
}
.grid-container {
  display: grid;
  grid-template-columns: 51% auto;
  gap: 4%;
}
.img {
  width: 100%;
}
.right {
  display: flex;
  flex-direction: column;
}
.title {
  font-weight: 600;
  font-size: 50px;
  line-height: 1.5;
  margin-top: 40px;
}
.content {
  margin: 20px 0;
  font-weight: 400;
  font-size: 20px;
  line-height: 1.5;
  opacity: 0.9;
}
.link {
  margin-top: 20px;
}
.Regist {
  font-size: 20px;
  color: var(--Violet);
  background-color: white;
  padding: 3% 10%;
  border-radius: 40px;
  width: 100%;
}

.Regist:hover {
  background-color: var(--Soft-Magenta);
  color: white;
}
.icon-container {
  text-align: right;
}
.icon {
  font-size: 40px;
  color: white;
  margin-left: 10px;
}
.icon:hover {
  color: var(--Soft-Magenta);
}

/*Responsive*/
@media (max-width: 400px) {
  .logo-container,
  .container {
    width: 85%;
  }
  body {
    background-image: url(images/bg-mobile.svg);
    background-repeat: no-repeat;
  }
  .logo {
    width: 60%;
  }
  .grid-container {
    display: block;
  }
  .left {
    margin-top: 7vh;
  }
  .right {
    text-align: center;
  }
  .title {
    font-size: 24px;
  }
  .content {
    font-size: 17.5px;
  }
  .content br {
    display: none;
  }
  .Regist {
    padding: 3% 20%;
    font-size: 18px;
  }
  .icon-container {
    margin-top: 100px;
    text-align: center;
    margin-bottom: 50px;
  }
  .icon {
    font-size: 30px;
  }
}
```

```js
const proudOfThisFunc = () => {
  console.log("🎉");
};
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
