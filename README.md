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

## Please don’t …
Yes, everybody understands that you don’t like the ‘fuzzy blue outline’ that surrounds an element when it is in focus in Chrome, etc. but please don’t remove it (or if you have to, replace it with the same outline, in another colour). 
Without this, nobody can see where they are tabbing and … well … it’s just naughty.

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
will always pay dividends over the bastardised 
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


## WAI-ARIA (Accessible Rich Internet Applications)
Simply put, Aria is a widely supported, accessibility supplement for browsers. It can be made to be ‘safe’ to allow it to degrade gracefully or encourage users to upgrade.
This has less of an impact on designers, but developers should commit to implementing it into their codebase from the very start of the project. 
Initially WAI-ARIA can seem daunting, but like everything else, it becomes easier with time.

_Visit this pages Wiki for examples._

## WAI-ARIA tips 
The trick is not to repeat yourself. If your markup features a <button> there is no need to add a role=”button”.  Semantics do the job.

## WCAG 2.0 Conformance Levels (A-AA-AAA)

WCAG 2.0 is divided into three conformance levels: A-AA-AAA
A should be described the absolute minimum, AAA it what you should desire.

Level A should have little impact on the design practice, AAA on the other hand will have.
The AAA Conformation Level can be described as the stickiest and most awkward of all the elements of accessibility. Consideration have to be made at the design level as colour and style will have a significant impact on obtaining AAA.

### Opinion
Simply put, AAA is a ruddy nightmare to satisfy. 
There are very few examples of a successful implementation of it on a commercially, but it isn’t something you shouldn’t aspire to.


> Conformance requirement #1 allows non-conforming pages to be included within the scope of conformance as long as they have a "conforming alternate version".
> ref: https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conforming-alt-versions-head

WC3 mention creating alternate versions of the site that meet the criteria and in most instances, this could be the only feasible way to go, to satisfy the requirements of the client, the designer and the poor bewildered developer.

_Visit this pages Wiki for examples._



