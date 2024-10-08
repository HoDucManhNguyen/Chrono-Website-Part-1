# Chrono-Website-Part-1

## Table of Contents

- [Purpose](#Purpose)
- [Essential Requirements](#Essential-Requirements)
- [Some Pictures of Product](#Some-Pictures-of-Product)
- [Link Demo](#Link-Demo)
- [Authors](#Authors)

## Purpose

This assignment will familiarise you with the techniques and skills involved in designing and creating static webpages utilising validated HTML and CSS created with a standard text editor. You will deploy these Web pages on a Unix / Apache server. This should be done in a way that keeps HTML content and CSS presentation separate.

## Essential Requirements

The Web site you will develop will describe a product/service for sale or hire.
It is up to you to provide details of the particular product or service and its features. Your Web site will have the following web pages linked by a common menu:
* An introductory / home page (index.html)
* A product description page (product.html)
* A product enquiry page (enquire.html)
* A page about your assignment (about.html)
* A page that lists any enhancements you have made (enhancements.html) </br>
You will also include:
* A CSS file that styles your website (style.css).

In general the web pages must:
* have relevant content
* include the HTML markup specified in the marking guide
* validate to HTML5 without errors
* have a &lt;head&gt; with Title, Meta tags as specified in template (including author)
* be styled by a validated CSS3 file
* be linked to each other via a menu 
* be deployed on Mercury

All web pages in your website should have a consistent layout and navigation. Where “in-house” templates have been defined in this unit (e.g. for meta-data; tables; etc.) these should be followed. These include accessibility alternatives.

The HTML in your Web pages must validate against the W3C HTML5 validator (http://validator.w3.org/nu)

Pages should not contain any deprecated elements/attributes (e.g. &lt;i&gt;, &lt;b&gt;). Do not use iframe elements in your assignment.

Note: Generic structural elements like div or span should only be used where there is no more meaningful HTML5 element (e.g. section) that is appropriate.

## 1. Introductory home page (index.html)

This page should contain appropriate header and graphic related to your allocated product, and should contain a menu that links to the other pages on your Web site.

This common menu should appear on every page of your website.

## 2. Product range page (product.html)

For example, the product you are allocated might be “restaurant meal”; or “SLR Camera”; or a “university course”.

The page must contain:
* Hierarchically structured headings of at least 2 levels
* More than one <section>
* An <aside> with appropriate content
* At least one appropriate image related to your product (This image should be less 100kb so it does not take too long to load)
* A table containing some data related to your product.
* At least one ordered list
* At least one unordered list
* At least one image

Your web page should describe a small range of products of this type (say 3 or 4). It is up to you to describe the details of the products. The products you describe can be real or imaginary. The products you describe must have a range of optional features from which the purchaser can select. For example, a restaurant meal could consist of a range of courses, with dine-in or take-away options etc. A camera might come in a number of models, with options of colours, lenses, etc.

You should write at least 150 words on the allocated product and its options. Appropriately structure the content with headings, paragraphs, lists etc. At least one product image must be included.
  
## 3. Product enquiry page (enquire.html)

This page has a form where a user can lodge an enquiry about a particular product. </br>
The form will have the following form controls:
* First name: type text , maximum of 25 characters, alphabetical only
* Last name: type text, maximum of 25 characters, alphabetical only
* Email address: type email
* Address (group these inputs with a fieldset and label)
  + Street address: type text, maximum of 40 characters
  + Suburb/town: type text, maximum of 20 characters
  + State: use a select list with options VIC,NSW,QLD,NT,WA,SA,TAS,ACT
  + Postcode: exactly 4 digits
* Phone number: type text, maximum of 10 digit. Use a placeholder
* Preferred contact: (email, post, phone). use radio.
* Product - from the range the user wants to enquire about. use select.
* Product features: use checkboxes
* Comment field, for example, allowing the reader to specify particular aspect they are interested in: use textarea, use a placeholder

All inputs should have labels. All form values, except the comment textarea are ‘required’ or have a default value (e.g. select, checkbox, radio). The user should not be able to submit the form if any of these required fields are blank. Use HTML5 validation to check the format.

***Data Submission to Server***

This form must have a Submit input. When this submit is activated, the name-values from the form will be sent to the server using the post http method. The server action address **https://mercury.swin.edu.au/it000000/formtest.php.** The server will then just echo back the name value pairs to the client. While nothing will be stored on the server in this part of the assignment, (we will do this in Part 3) this will allow the form to be tested.

## 4. A page about you (about.html)

This page will contain your details.

The following information should be structured with a definition list and formatted appropriately. For example:

Name: Amy Smith
Student ID: s1234567
Course: Bachelor of Science
Email: 1234567@student.swin.edu.au

The following information should also be included and formatted accordingly:

<img width="1166" alt="Screenshot 2024-09-06 at 9 31 43 PM" src="https://github.com/user-attachments/assets/a337b4f3-25b4-4b81-bcca-501c924c0bfd">

It could also include personal profile, such as resume, interests, or information that is related to you. This extra information gives you an opportunity to extend the techniques you apply in your assignment, and could include:
* Demographic information about you
* Description of hometown
* A list of your favourite books, music, films etc

## 5. CSS Requirements

***No style markup should be included in your HTML file.***

The pages in your web site must be styled with CSS and have a consistent ‘look and feel’, particularly with markup of menus, headers and footers. While the emphasis in this assignment is on the appropriate application of techniques rather than graphic design, your pages should follow basic usability / accessibility principles, e.g. distinguishable foreground and background colours, and font readability, etc.

You are to create your own single external stylesheet to implement your design.

1. CSS should be commented at the beginning of the CSS file to identify author and purpose, and individual line comments should be used as necessary to explain particular styles and explain where they are applied.
2. All the following CSS Selectors should be used appropriately at some point in your assignment:
   * element, #id, .class, grouping, contextual
   * pseudo class or element
3. Provide appropriate formatting to your menu with a background colour.
4. The following specific CSS rules should be demonstrated on your index.html page:
   * display a background graphic.
   * the footer text should be in a small font and centred in the footer
5. The following specific CSS rules should be demonstrated on your product.html page:
   * &lt;h1&gt; elements should have their font variant, size and family etc. set using the short-hand font property.
   * The table should have one background colour for the headings and another background for the data cells
   * The &lt;aside&gt; should be 25% of the width of page and float to the right.
   * The &lt;aside&gt; should have a coloured border with an appropriate margin and padding.
   * The footer should cover the full width of the page.
6.All pages should have a fluid layout (the page should “Reflow” on page resize).

Other CSS selectors and properties can also be used if deemed necessary and appropriate for the presentation. Your menu should have its own set of styles applied. CSS should be commented at the beginning of the CSS file to identify author and purpose, and individual line comments should be used as necessary to explain particular styles and explain where they are applied.

For this assignment you should create one single CSS file that applies to all your Web pages. This file should be named style.css. You can use another CSS file for enhancements.

> [!TIP]
> CSS validators will validate against a particular version of CSS e.g. CSS2.1 or 3. This assignment should be valid CSS3. Make sure that you are checking your CSS using the correct version of the validator. For example, if you include CSS3 markup and validate as CSS2.1 it will show errors. Do not include any proprietary CSS mark-up, such as –moz- or –webkit- etc.
 
## Enhancements

> [!WARNING]
> Make sure you get all the basics working first before you attempt any enhancements.

The technologies for developing Web applications are rapidly changing. One of the key skills you will need is finding out about these techniques (from the Web) and applying them. This assessment gives you an opportunity to demonstrate your ability to implement features/techniques that go beyond the specified requirements above. This is an opportunity to demonstrate your ability to discover techniques from a range of sources and apply them in a standards compliant manner.

These enhancements need to be implemented within the Web pages (index.html, product.html, enquire.html, about.html). The extra feature needs to enhance your Web site in a relevant way.

On a separate Web page called enhancements.html list and describe each enhancement you have made and how you have significantly extended the basic HTML and CSS beyond what is covered in the Tutorials. Hyperlink from this list to where the feature is implemented in your Web site. If it is a CSS feature, hyperlink to an example of the html that is selected by the CSS rule. For each enhancement feature briefly explain:

- [x] how it goes beyond the basic requirements of the assignment
- [x] what code is needed to implement the feature
- [x] if you have sourced your technique from a third party the source of this technique (e.g. URL) must be cited.
- [x] a hyperlink to where you have applied that extension in your Web site (this is needed so the tutor can quickly assess your enhancements).
- [x] All enhancements must be able to run on Firefox or Chrome. Make sure you check this.

A maximum of 2 enhancements will be assessed (up to 10 marks each). Examples of HTML/CSS enhancements include:
* Effective, appropriate and innovative use of a number of distinct HTML elements not covered in tutorials (e.g. Image maps) used in a way that improves the user experience of the website.
* A number of additional CSS properties or selectors (e.g. support for interactivity) not covered in the tutorials. For example the use of a range CSS3 pseudo-elements and classes, child or siblings combinators, attribute selectors, etc.
* Implement Responsive Design with additional CSS that presents your website specifically for mobile phone / tablet sized displays.
* In addition to you standard CSS, create another CSS files that re-implements and extends the style with a library/preprocessor such as Bootstrap, LESS or Sass. Demonstrate and document a number of cool features that can be implemented using the library.

Discuss your proposed enhancements with you tutor before you implement them. The number of marks you receive for an enhancement will be at the sole discretion of your tutor/marker. As a guide if the enhancement has only taken a couple of lines of code it is likely to be trivial.
* Be relevant to / enhance the content of the website
* Be well described (as explained above)
* Be non-trivial.
* Be significantly different from other features you have implemented.

> [!CAUTION]
> Do not include JavaScript in this part of the assignment.


## Web Site Folder Structure and Deployment

Create a website structured as described below. You can create additional HTML files for your content (depending on what your content requires), but the following is needed:

<img width="1166" alt="Screenshot 2024-09-06 at 9 45 13 PM" src="https://github.com/user-attachments/assets/7119c458-059c-41c0-a3f9-b42b448b6813">

***Notes:***
* HTML files should only be in the base “assign1/” folder – not anywhere else.
* All images used for the content should be stored in the “assign1/images/” folder.
* All images used for the style should be stored in the “assign1/style/images/” folder.
* There should be a “style.css” file in the “assign1/styles/” folder.
* All links to your files (CSS or images) should be relative. Do not use absolute links, as these links will be broken when files are transferred for marking. No marks will be allocated if links are broken.

## Some Pictures of Product

<img width="1280" alt="Screenshot 2024-09-06 at 9 47 18 PM" src="https://github.com/user-attachments/assets/5da4a285-a95c-4803-a58e-8455c8d071b4">

<img width="1280" alt="Screenshot 2024-09-06 at 9 47 46 PM" src="https://github.com/user-attachments/assets/5b712fbe-402f-4061-8a23-f75fdc1a5d67">

<img width="1280" alt="Screenshot 2024-09-06 at 9 48 08 PM" src="https://github.com/user-attachments/assets/ea2119ed-33b2-4598-b331-8e30b1382504">

<img width="1280" alt="Screenshot 2024-09-06 at 9 48 24 PM" src="https://github.com/user-attachments/assets/36b00840-8eec-469f-8829-c275b8e66ea3">

<img width="1280" alt="Screenshot 2024-09-06 at 9 48 48 PM" src="https://github.com/user-attachments/assets/58e89a6c-c5ae-4aaf-8dda-74b750e644f0">

<img width="1280" alt="Screenshot 2024-09-06 at 9 49 15 PM" src="https://github.com/user-attachments/assets/2cbb845c-e979-444d-96b1-94d81e6666d3">

<img width="1280" alt="Screenshot 2024-09-06 at 9 49 32 PM" src="https://github.com/user-attachments/assets/dd99e6a1-952d-466b-b2f8-2d298a625d9e">

<img width="1280" alt="Screenshot 2024-09-06 at 9 49 51 PM" src="https://github.com/user-attachments/assets/1b3c9a80-485f-4746-8287-3f770a1f3352">

<img width="1280" alt="Screenshot 2024-09-06 at 9 50 12 PM" src="https://github.com/user-attachments/assets/6f663de9-0a5c-438a-ba5a-4b49d458c9c0">

## Link Demo
https://hoducmanhnguyen.github.io/Chrono-Website-Part-1/product.html 


## Authors

Name: Manh Nguyen (Harry) </br>
Email: manhnhd.vn@gmail.com </br>
LinkedIn: https://www.linkedin.com/in/harrryy/

