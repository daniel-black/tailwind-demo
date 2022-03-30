# Tailwind CSS
- CSS library 
- Provides a constrained set of primitive utilities

Similar to how a programming language defines a set of primitives like `int`, `string`, or `boolean` that allow you to compose pieces of logic into a program, Tailwind gives you a set of styling utilities that can be applied to HTML elements as classes.

----

### Traditionally, styling looks like this:

```html
<div class="chat-notification">
  <div class="chat-notification-logo-wrapper">
    <img class="chat-notification-logo" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div class="chat-notification-content">
    <h4 class="chat-notification-title">ChitChat</h4>
    <p class="chat-notification-message">You have a new message!</p>
  </div>
</div>

<style>
  .chat-notification {
    display: flex;
    max-width: 24rem;
    margin: 0 auto;
    padding: 1.5rem;
    border-radius: 0.5rem;
    background-color: #fff;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  }
  .chat-notification-logo-wrapper {
    flex-shrink: 0;
  }
  .chat-notification-logo {
    height: 3rem;
    width: 3rem;
  }
  .chat-notification-content {
    margin-left: 1.5rem;
    padding-top: 0.25rem;
  }
  .chat-notification-title {
    color: #1a202c;
    font-size: 1.25rem;
    line-height: 1.25;
  }
  .chat-notification-message {
    color: #718096;
    font-size: 1rem;
    line-height: 1.5;
  }
</style>
```
**Result:**
![chitchat component](readmeAssets/chitchat.png)

**Process**
- Define the structure (HTML)
- Spend entirely too long coming up with abstract class names like `search-result-blob-wrapper`
- Divine from the seemingly endless set of CSS properties which precisely will be needed to style your elements, all the while trying to take advantage of the cascading property of CSS.

---

### Lets see how we can do this with Tailwind CSS!

[Bare bones HTML](https://play.tailwindcss.com/6QVsPG2z0I)
[Styled component](https://play.tailwindcss.com/tKhde0Z6mk)


**Key points**
- Never have to leave the HTML
- Don't need to name things
- Ask and you shall recieve (If I want a component to have rounded edges I just say "Hey tailwind, make it `round`")

**Elephant in the room...** Okay yes, it is ugly *but* just bear with me for a moment here.

---

### This kinda feels like inline styling??
We can do animations just by applying a class or two

Lets make a button pretty and animate the hover effect 

[Button Start](https://play.tailwindcss.com/y6Bo6w4cP3?layout=horizontal)
[Button Final](https://play.tailwindcss.com/ZdZrmaMi6k?layout=horizontal)


Card Loading animation
[Starter](https://play.tailwindcss.com/qvoocbtOom)
Just add `class="animate-pulse"` to the div with no classes

Dark Mode (change mode on your device)
[Finished](https://play.tailwindcss.com/3ag4SpnMH0)

[Animated Notification](https://play.tailwindcss.com/khqX4PVxmN)

[Not sure what to call this but its cool when you hover](https://play.tailwindcss.com/h1dydlAK1x)

[Responsive Card](https://play.tailwindcss.com/T3bloxI4z8)

[Responsive Cards](https://play.tailwindcss.com/V6nOlDpq4U)

[Lite clone of linear.app](https://play.tailwindcss.com/3X8XP5eBgc)
