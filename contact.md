---
layout: page
title: Contact
permalink: /contact/
menu: true
---
<form action="" name="contact" method="post" enctype="text/plain">
  <p>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name"
      placeholder="Please provide your name">
    <label for="company">Company:</label>
    <input type="text" id="company" name="company"
      placeholder="Please provide your company">
  </p>
  <p>
    <label for="phone">Phone:</label>
    <input type="tel" id="phone" name="phone"
      placeholder="Phone">
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required
      placeholder="Email">
  </p>
  <p>
    <label for="subject">Subject:</label>
    <input type="text" id="subject" name="subject" required
      placeholder="Subject">
  </p>
  <label for="message">How can we help you?</label><br>
  <textarea id="message" name="message" rows="5" required
    placeholder="How can we help you?"></textarea>
  <p>
    <input type="submit" value="Send">
  </p>
</form>
