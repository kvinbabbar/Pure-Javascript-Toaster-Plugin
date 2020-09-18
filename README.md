# Pure Javascript Toaster #
*Requires Nothing*

[**Demo**](https://kvinbabbar.github.io/Pure-Javascript-Toaster-Plugin/)

**Toaster** is a Pure Javascript plugin for displaying toast notifications. It comes with different options e.g custom text or HTML message, duration, custom class, toggle close button, position, custom close icon and backgorund color.

### What Is This Toast You Speak Of? ###

While *toast* is most often used to describe sliced bread that has been browned by dry heat, it can really refer to any kind of material that has been browned in such fashion.

Or - as is our case - toast can refer to a **non-modal**, unobtrusive UI element used to display brief, **auto-expiring** (aka auto-dismissing) windows of **information** to a user. It does not accept focus or user input, nor does it interrupt the current activity.

>While the definitive origin of the term "toast" to describe this type of notification system is unknown to me, it could reasonably be a reference to either (a) the salutation or words of congratulations, good wishes, appreciation, etc., spoken immediately before drinking to a person or event *or* (b) the fact that it pops up like bread from a toaster. Cheers!

## Usage ##

Include the `toaster-box.js` JavaScript file and `toaster-box.css` CSS file on your HTML page, then display toast messages anytime like this:

```javascript
/*
* Pass an parameters as an object:
* The only required paramter is message
* Order does not matter
*/
new ToasterBox({ msg : 'Your message here' });
new ToasterBox({ msg : 'Your message here', duration : 3000 });
new ToasterBox({ msg : '<strong>Success</strong> Your message here', html : true, closeButton : false });
new ToasterBox({ msg : 'Your message here', maxWidth : 350, position : 'top-right' });
new ToasterBox({ msg : 'Your message here', autoOpen : false, closeIcon: '<i class="fas fa-close">' });
new ToasterBox({ msg : 'Your message here', className: 'custom-class' });
