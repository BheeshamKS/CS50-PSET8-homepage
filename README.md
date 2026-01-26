# CS50 Problem Set 8 - Homepage

This repository contains my solution for the "Homepage" problem from Harvard's CS50 course. The project involves creating a comprehensive, multipage personal portfolio website using HTML, CSS, JavaScript, and the Bootstrap 5 framework.

## Links

- **Live Site:** [https://bheeshamks.github.io/CS50-PSET8-homepage/index.html](https://bheeshamks.github.io/CS50-PSET8-homepage/index.html)

## Files

`index.html` : The landing page containing the "Hero" section, introduction, and navigation to other areas of the site.

`projects.html` : A gallery page displaying my work in C, Python, and UI Design using responsive Bootstrap cards.

`about.html` : A personal page detailing my background, including interests in Operating Systems, 3D Animation, and Coding.

`contact.html` : A functional interface allowing users to send messages via a simulated form and view social media links.

`styles.css` : The custom stylesheet that overrides Bootstrap defaults to create the "Dark/Teal" theme, floating card layout, and animations.

## Description

The website is designed with a unified "Dark Mode" aesthetic (Deep Charcoal & Electric Teal) and demonstrates mastery of grid layouts and responsive design:

- **Global Navigation:**
  - A consistent Bootstrap Navbar is present on all pages.
  - Features a custom FontAwesome hamburger menu for mobile devices.
  - The "Active" state highlights the current page link in Electric Teal.

- **Responsive Layout:**
  - **Desktop:** The content "floats" in the center of the screen with a 50px margin, creating a modern card effect.
  - **Mobile:** Media queries remove the margins and stack the content vertically to utilize the full screen width.

## Output Behavior

The page utilizes CSS transitions and JavaScript to provide immediate visual feedback:

- **Loading State:**
  - Upon opening any page, a JavaScript event listener triggers a full-screen overlay with a spinning teal loader.
  - Once the DOM is fully loaded, the overlay fades out to reveal the content.

- **Hover Effects:**
  - **Buttons:** Hovering over the "Hire Me" button transitions the background from Teal to White.
  - **Cards:** Project cards and the "About" section feature subtle shadow enhancements to create depth.

- **Form Interaction (Contact Page):**
  - Users type their Name, Email, and Message into the dark-themed inputs.
  - Upon clicking "Send Message", JavaScript intercepts the default submission.
  - An alert box appears confirming the message was sent, and the form resets automatically.

## Example Interaction

**Navigation Flow:**
User loads `index.html` -> Loader spins -> Page fades in.
User clicks "Projects" in Navbar -> Navigates to `projects.html` -> "Projects" link turns Teal (Active).

**Contact Form:**
User types "Hello World" in the message box.
User clicks "Send Message" -> Browser displays alert: "Message Sent! Thank you for contacting me."
User clicks "OK" -> Input fields are cleared.

**Mobile Responsiveness:**
User resizes browser to phone width -> The "Hello" text and Profile Image stack vertically.
User clicks Hamburger Icon -> Menu slides open.
