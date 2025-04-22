# UX-Assignment-3 Project

## Project Overview

This repository contains a collection of responsive HTML5 web pages which implement three Figma wireframes I've created for my UX assigment.
The web pages are meant to work seamlessly across dekstop, mobile and tablet devices of all sizes. 
The goal of this project is to learn how to transform wireframes into responsive front-end user interface using HTML5, CSS3, and frameworks.
In addition to that this project focuses on information architecture, uses GitHub for version control and GitHub Pages for deployment.
For this project I've used Bootstrap framework.

---

## What This Project Does

- Contains three responsive HTML5 pages which implement 3 user stories and index.html page for navigation.
- Contains shared styles.css file with custom styles shared across all three pages like colours, customised text inputs, buttons etc.
- Uses Bootstrap framework (https://getbootstrap.com/) to implement layout responsiveness.
- Uses semantic HTML5 tags like header, footer, main, article, section in order to enhance accessibility and make the pages ready for search engine optimisation.

---

## User Stories

The three pages I've created implement three user stories I've come up with in the UX Assignment 2 and are meant to offer users three valuable features on the coffeeshop website such as:
- store locator page;
- order summary page;
- order delivery options page.

### User Story 1: Store locator page

- As a: **mobile office worker**
- So that: I could save time on grabbing coffee from a coffeshop at lunch time
- I need: website to allow me to locate nearest coffeshop I could make my online order from

**Acceptance criteria:**
- User has access to the store locator on the website
- Use can enter post code into a text box and get the list of 5 nearest coffee shops to his post code
- There has to be a list of 5 nearest coffee shops to be shown to a user with their names, addresses,  distance to them, closing time and delivery options.
- All 5 nearest coffee shops have to be shown on the google maps for user to be able to understand where they are located and provide visual guidance how to find them.
- The text content on the page is accessible with big enough text and in high contrast to help visually impaired users.

### User Story 2: Delivery options page

- As a: **mobile office worker**
- So that: I could save time on grabbing coffee from a coffeshop at lunch time by making online order and get it delivered to me.
- I need: website to allow me to pick the delivery option and use it for my online order

**Acceptance criteria:**
- User can select the delivery service from Deliveroo, UberEats, JustEat.
- Use can enter details for the delivery service such as first name, last name, delivery address, contact email/phone number.
- User can select a time slot convenient for them for the order to be delivered.
- User can enter optional comments for the delivery service e.g. "The bell does not work, please knock on the door."
- User must be able to confirm order by clicking the button "Order Now".

### User Story 3: Order summary page

- As a: **student**
- So that: I could save time in the morning when picking up my coffee from the coffeeshop by making order on the bus through the app
- I need: App and website to allow me to view my online order to check its content and everything looks right and then proceed to checkout

**Acceptance criteria:**
- User can see the items they chose in the menu and the price for each item and quantity.
- Use can see the subtotal of all items a user added to the order, VAT amount for the order and the total amount with VAT to be paid during the checkout.
- User can click 'Proceed to checkout' button to get to the checkout page to enter payment information.
- User can click 'Back to menu' button to get back to the menu page where additional items can be chosen to be added to the order.
- Text should be accessible as the user has dyslexia.

---

## Development Process

### Wireframes

The feedback from Assignment 2 Group Project was this:
"Wireframes design are clear completed for both desktop and mobile view port. Showing clear sample content. Some evaluation of designs based on usability and accessibility."

Based on the above feedback no major changes were done to the Figma wireframes I've created. 

However, for the responsive front-end user interface I've decided to further enhance usability and accessibility by introducing the following things:
- Buttons highlightting so that when a user hovers mouse over a button on a page it changes its colour;
- Add placeholder text to the text inputs to guide a user what input is expected in each text input;
- Add highlighting to a delivery partner image when mouse mouse hovers over it to visually guide user which option is selected;
- Add contrast border and shadow to text input fields and buttons to make them visually stand out for users;
- When mouse hovers over a hyperlink in the header menu or footer menu the text becomes underlined to visually inform user which hyperlink is selected.

![Store Locator Page Wireframe Desktop Version](docs/wireframes/store-locator-wireframe-desktop.png)
![Store Locator Page Wireframe Mobile Version](docs/wireframes/store-locator-wireframe-mobile.png)
![Order Summary Page Wireframe Desktop Version](docs/wireframes/order-summary-wireframe-desktop.png)
![Order Summary Page Wireframe Mobile Version](docs/wireframes/order-summary-wireframe-mobile.png)
![Delivery Option Page Wireframe Desktop Version](docs/wireframes/delivery-option-wireframe-desktop.png)
![Delivery Option Page Wireframe Mobile Version](docs/wireframes/delivery-option-wireframe-mobile.png)

### Information Architecture

In order to facilitate easy access to different pages index.html simple page has been added to implement main navigation menu to navigate between all three responsive pages.

To ensure a structured and logical layout and to enhance user experience and usability each of the three responsive page and index.html have the same logical layout:
- header section with the coffeeshop name Brewtopia and navigation bar with hyperlinks to other pages of the website e.g. Home leads to index.html and Store Locator leads to the corresponding responsive page.
- main/middle section of the page with the responsive content of the corresponding page;
- footer section with another set of hyperlinks and also copyright info which is usually being added onto websites;
- the main section of the order summary page is organised with top down information flow in mind so that a user goes from top through each order item and for each order item from left to right and then comes down to the order totals and finally to the bottom where two Back to Menu and Proceed To Checkout buttons are present. Same top down flow is implemented for mobile version;
- the main section of the delivery options page is also organised with top down information flow where a user starts at the top by selecting one of three delivery partners and then continues down by filling in delivery details and finally coming to the bottom with the order total amount being shown to recap it to a user and Order Now button being present. Same flow is followed for the mobile version;
- the main section of the store locator page has search text input on top to allow a user to enter search query and then list of found coffeeshops on the left side and the main element being the map with found coffeeshops on the right and it takes the 80% of the screen size. For the mobile version after the search text input the map goes first as it has better accessibility
 for users comparing to textual output and then list of found coffeeshops goes.


### Project Design Considerations

When designing the project I've considered the following things:
- all file names and folder names mustt be in lower case. That's because when they are being deployed likely it is going to be a Linux server so file names and folder names are case sensitive;
- all the files in the project have to be organised into a logical folder structure.

## Code Organisation

The code is meant to be clean, readable, and maintainable with meaningful variable and function names and I am aiming to achieve this by:
- variables are used in CSS for colours so that if I need to change a color value say for a header I change one variable and changes are applied everywhere where this variable is used;
- UI elements have meaningful names;
- every attempt is made to make code shared across pages like for example same code is used on all pages for the header and the footer;
- single styles.css file is used to contain all of the CSS code which can be reused on all pages and maintained in a single place.

Follow consistent code formatting and style guidelines:
- indentations are used in HTML to clearly isolate blocks of code into a hierarchy and enable quick navigation throughout the code;
- empty lines are used in the files to additionally separate logical blocks of code e.g. main section from header and footer from the main section;

Use comments and documentation to explain complex logic and provide context:
- HTML code is documented with comments throughout providing the context what is being rendered in each logical block of code;
- styles.css file with CSS code has comments throughout.


## Folder Structure 

├── index.html
├── store_locator.html
├── delivery_options.html
├── order_summary.html
├── README.md
├── css/
│   └── styles.css
├── docs/
│    ├── wireframes/
│	 │	 ├── store_locator_wireframe_desktop.png
│	 │	 ├── store_locator_wireframe_mobile.png
│	 │	 ├── delivery_option_wireframe_desktop.png
│	 │	 ├── delivery_option_wireframe_mobile.png
│	 │	 ├── order_summary_wireframe_desktop.png
│	 │	 └── order_summary_wireframe_mobile.png
│    └── screenshots/
│	 	 ├── store_locator_final_desktop.png
│	 	 ├── store_locator_final_mobile.png
│	 	 ├── delivery_option_final_desktop.png
│	 	 ├── delivery_option_final_mobile.png
│	 	 ├── order_summary_final_desktop.png
│	 	 └── order_summary_final_mobile.png
└── assets/
     └── images/
		 ├── map.png
		 ├── uber_eats.png
		 ├── deliveroo.png
		 ├── just_eat.png
		 ├── coffee.png
		 ├── sandwich.png
		 └── cake.png

