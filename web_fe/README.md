Front End Developer Coding Test
===============================


### Instruction

> Please implement a web form that used on mobile device with following features. Visual design is provided as attached images:

### Feature Requirements

* Implement validation for user-name field. If empty string or only empty space provided, it should break submit process, and display validation error as design shown.
* Encryption is a switch-box.
  * Transition animation is required
  * Please try to implement it as mush less html elements as possible
  * If possible, try to avoid javascript to implement switch-box
  * Its value should be submitted if switched on
* Password value should be encoded before submit to server
  * To simplify the problem, you can use `Base64` as encoding algorithm ( Yep, Yep, Base64 isn't an encryption algorithm. If you have better idea, please do it as your wish. )
  * Please do use a library rather than implement your own encryption algorithm.
  * You might find useful stuff on https://cdnjs.com/
  * The original value should never be sent without encoded.
* Password field should be controlled by encryption switch
  * Password field should not be shown unless encryption switch is on
  * Password field should not be submitted when encryption is off, even password has value filled in before
  * Password field should remember its value when encryption switched off and on again.
* Price field has fixed currency prefix, and fixed suffix `.00`
  * Euro is used in visual design. But you can have any currency prefix as your wish, bit-coin maybe
  * Glyph-icon might be helpful to implement this.
  * The price field should yield validation error if non-number value is provided.
* Please submit the form via ajax
  * Make the submit button to `busy` mode during uploading
  * Submit should be triggered when a previous uploading is not yet finished

### Technical Requirements

#### 1. General

* Page is only used on mobile device, desktop can be ignored.
* Responsive is encouraged but not mandatory.
* Consider modern browsers only, do not worried about all kinds of IE!

#### 2. Html

  * Make you Html clean and organized
  * Make sure you Html is compatible with Android and iOS devices
  *

#### 3. Stylesheet

  * You can use Grid system or similar CSS framework to help you on alignment.
  * Write your own CSS to decorate your components. **DO AVOID** to use CSS component provided by frameworks, such as Bootstrap
  * You can use CSS-Preprocess language, such as LESS, SASS or Stylus. And **DO PROVIDE** a compiled CSS file if you use them.

#### 4. JavaScript

  * You can use JavaScript library to help you on DOM manipulation, such as jQuery, Angular, React, Backbone, Knockout, Vue or any other library you like.
  * Write your own JavaScript interaction components. **DO AVOID** to use components provided by library, such as Bootstrap Js Components, jQuery plug-in that enhances inputs.
  * ES-hamony features are encouraged, use `Babel` or other spoilers you familiar with.  

#### 5. Clean code

  * Try you best to make your code clean, all kinds of lints are recommended.
  * Try to organize your stylesheet and javascript structured and organized.
  * We loves bug-less code, so automation tests should be highly praised!
