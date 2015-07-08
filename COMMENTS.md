
Assignment Feedback:

The overall code looks great. Here is a summary of the feedback mostly just optimization issues.

-----------
HTML
-----------

1. The <logo> tag is not part of the standards. Please use the anchor tag, <a> for logos. Please note that logos are commonly used as links to the homepage from the internal pages.

2. Please use the parent tags to help select the child elements. This way is cleaner, e.g. the classes '.header-logo' and '.footer-logo' can be replaced ny the selectors : 'header .logo' and 'footer .logo'. This way bith logos can share the classname '.logo'

3. Please avoid using the <br> tag  for the page layout. This is best used for the text content.

-----------
CSS
-----------

1. Using fixed heights for the sections can be a problem should especially if the content is dynamic. 'min-height' would be a good alternative. That way if the content changes, the section will just grow in height.

2. I noticed that the font family rule "font-family: 'Open Sans', sans-serif;" has been used on several elements. It might be better to make the rule more global so you dont have to keep repeating it in the css.
 e.g 
	body{
		font-family: 'Open Sans', sans-serif;
	}

3. Please also look into using padding in the container element instead of margin in the child elements where possible. 
	e.g. putting a padding of 80px in the <header> would make it easier to position the contents away from the border rather than having to place margins on every child element.

	Please also look at using {margin: 0 auto} to center child elements. {text-align:center} may work sometimes but this is usually meant to center text content. using the {margin: 0 auto} also lets you select only the block elements you want to center. 
	
	Please review the positioning of some elements (e.g the logo in the header). I will be happy to answer any questions regarding the use of padding, and margins. 

	Please let me know if you want to discuss this further. 

