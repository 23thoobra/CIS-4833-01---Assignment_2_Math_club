CIS 483/583 - Homework 2: Maverick Math Club Website
Author: Braden Thooft
Github Link: https://github.com/23thoobra/CIS-4833-01---Assignment_2_Math_club

I wrapped the main menu in a <"nav"> element instead of a generic <"div">, because <"nav"> tells screen readers and search engines that this block is the site's main navigation, so a screen-reader user can jump straight to it. In the events table I used <"th scope="col""> for the column headers and <"th scope="row""> for the dates, so a screen reader reads each cell along with its column and date instead of a meaningless stream of text. I also put the club news in an <article> because it would still make sense on its own, and the "Math Question of the Week" in an <aside> because it is related to the page but not part of its main content. 

When I opened my pages with the DevTools Console open, both images were broken and the Console showed red "Failed to load resource" errors. The cause was wrong image paths: on the home page I wrote src="logo" and src="chalkboard.jpg" without the images/ folder or the logo's .png extension, and on the events page I had a typo, src="imagesg/logo". I fixed them by changing the paths to images/logo.png and images/chalkboard.jpg so they matched the real file names and folder exactly. The validator also caught a broken checkbox tag that was missing its closing > and its name attribute, which I fixed by completing the tag. After these fixes both pages had zero validator errors and zero red errors in the Console.

Sources:
- MDN Web Docs, HTML elements reference: https://developer.mozilla.org/en-US/docs/Web/HTML/Element
- MDN, Client-side form validation: https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation
- W3C Markup Validation Service: https://validator.w3.org/
- W3C Markup Validation Service: https://validator.w3.org/
