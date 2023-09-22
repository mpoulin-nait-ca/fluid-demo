# Build Methodology


## HTML

1. Start by sectioning everything off and migrating all of the body copy from the provided markdown file to the markup. You should have a header with navigation and a hero banner, a main with three sections, and a footer.

2. If you'd like to use on-page anchors, you can create an ID for each section and link to it in your navigation. You can also prepend the hyperlink references in your footer to modify the browser's behaviour, giving the telephone number and email address a little added functionality. Validate your code.


## Utility Classes

Utility classes are a way of writing modular code -- that is, they are a set of rules that can be used over and over again on multiple elements.

3. Hop into your CSS and write a simple .container utility class. This .container class will keep your layout from growing beyond a certain width; however, we still want to have full-width background colours and a full-width background image for our hero banner. Your challenge will be to figure out how to constrain your content while still allowing backgrounds to span the entire viewport.

> Hint: wrapping all of your content in a div.container like we did in COMP1017 will not work.

4. We want to add a little bit of padding to every element with a .container class to give it a little more vertical white space; however, we do *not* want to include the navigation, as we want to keep it relatively short. What are some ways we could target everything *except* the navigation? 

> Hint: you could use classes, or an extensive multiple element selector. But you could also use a :not() to create an exception to your rule.

5. Create a .flex class and apply it to every element that you want to turn into a flex container. 


## More CSS

6. Using top-down logic, begin with more general or universal styles and get gradually more specific. Start with typographic styles, then get into individual sections.

7. When you get to the hero banner, your challenge will be to create a full-screen banner that responds to the viewport width and height; the vw and vh units will allow you to do this. However, the navigation is already taking up a little bit of the height on your screen; how can you make sure that you account for this height and not create any overhang?

> Hint: try using the element inspector to figure out the height of your navbar and subtract this from the total viewport height using the calc() function.

8. Finally, while it's convenient to use flexbox to shove flex items into the middle of a container, you do not always want things in a row. Which property can you use to arrange your heading and paragraph in a column once more?

9. Continue to work with your instructor through the rest of the page. As you work, continue to make sure that your layout looks good regardless of the viewport width by resizing your browser window.