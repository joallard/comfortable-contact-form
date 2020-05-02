# The Comfortable Contact Form
(until I find a better name!)

![](https://github.com/joallard/comfortable-contact-form/raw/master/image.png)

For asynchronous communication between your visitors and you.

* Using a contact form as a visitor is full of friction and never very fun.
* Implementing a contact form is a pain and one more thing to bother with

I've been forever dissatisfied with the current solutions.

In my website mockups, asking a question is always designed to be easy and encouraged. It is not so.

Not anymore.

Your visitor talking to you should be a smooth, pleasant experience. It should be as easy as asking a salesperson a quick question.

As a developer, you should drop one line in your code and be done with it. It should have good defaults which you can customize.

## Usage
Choose your own level of bothering, from minimal to hands-on.

Custom elements approach:

```html
<contact-form-dialog></contact-form-dialog>
```

And then:
```js
document.querySelector("contact-form-dialog").open()
```

And that's it.

Or use a macro:

```haml
= contact_form_dialog
```

Will also be available: integration in React or Vue.

### Options
Dialog:
* action (`POST /submissions`)
* locale (`<html>.locale`)

Open:
* context (`<title>`)

### I18n
Enough of second-class, time sink I18n. Just works by default, batteries included.

### Styling
Uses `--accent-color` as the accent color. (Leaving empty: minimal black and white)

## Design methodology
It should be constantly optimized for humans, never the reverse.

We should make the user as happy as possible, the developer as happy as possible, and the staff as happy as possible.

### Little details
* Button hit zones are large enough for fingers
* Focus on communication first, details after
* It is a dialog on the page and doesn't obscure the context
* It saves automatically, and persists from page to page
* It remembers you, but will happily forget you if you ask
* You can take as few or as much space as you want to write
* You can edit your answer
* You can save it for later, or discard altogether and start over (and undo!)

* Context can be programmatically added

### CSS
You can include as much or as few CSS as you wish:
* None: No CSS.
* Minimal: The CSS it takes for it not to look broken, nothing more. Equivalent of default HTML styles.
* Themed: The whole enchilada, ready to go. Includes niceties like border-radius and some font-weights. Define `--accent-color` and you're good to go!

## Todo
* Dark background
* Accessibility tags
