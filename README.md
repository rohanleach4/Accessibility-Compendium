# Accessibility - Compendium
## A thoughtfully composed suite of opinions and best practices for Designers and forgetful Developers

## Where does accessibility start?
Accessibility doesn’t start with developers. It starts at _the start_ of the project, at the top of the pyramid. 
Accessibility, at the very least should be baked into the culture of the company producing the product.
The first physical implementation of accessibility will probably be at the design stage.

## Designers vs. Creatives

> ### Designers are more aligned to architects,
> ### Creatives to artists
> #### - Alexa: Queen Bitch

A good design has to be fit for purpose. It has to be fit for all the mediums it is going to be viewed on. 
In the case of designing for a digital medium, whether in a browser or a native app, the easiest way to ensure this will happen is to pay attention to the semantic layout. If you do this, you cater for all users, regardless of ability. 

## Be equitable in your design
It has been noted that 1 in 5 people can be described as having a disability.
Make sure it can be viewed and enjoyed by everyone, regardless of their ability.
Do this and the world will be a better place … and … it’s the law.

## Conclusion
A good designer will always deliver a more robust and useable product than a great Creative.
The world needs more Designers.

## Janet and John stuff
Make every effort to be semantically correct throughout the design. 
This is simple.
This is almost 80% of the battle.

Using appropriate tags like:
```html
<button>This is a button</button>
<input type=”text” />
```
will always pay dividends over bastardised 
```html
<div tags type=”button” role=”button”>Try and tab this ya bugger</div>
<div contenteditable="true">Please Die if you use this</div>
```
If you use the correct tags, the user can tab between the elements and use the return key. 
It works across all browsers and doesn’t require any JS to sort its nonsense out. 
Appropriate tags are a web standard.

Semantics don’t just end with buttons and input fields.
h1, h2, h3, h4, h5, p tags are equally important.
These help screen readers.

Semantically correct sites are going to be lighter in weight (most, if not all of the functionality is done for you), better for mobile ands probably, although I am loathed to say this, better for SEO.

## Testing

When building a digital product, in this instance a website, get in the habit of testing as you go along. It doesn’t take very long and once you get in the habit of doing so, it just feels natural and you won’t have to go back and rewrite it later.

> #### You never add accessibility to a site at a later date.
> #### You rewrite the site and do it properly.
> #### What’s the point? Do it right first time.

### Testing tools
If you use Chrome, go to Audits (this used to be called Lighthouse before it was baked into the browser) and run an audit. 
This will audit your site and give you an accessibility score.
Never accept anything less that 100/100. 
This isn’t the be-all-and-end-all of accessibility. With this score, you have something to build on.

Every time you view a change or update to your site, check that every element can be tabbed with the tab key. It is essential that this works. If it doesn’t, stop and fix it. Don’t pile more code on top of a broken page.
Make it a part of your work ethic and you will save loads of time later on.



