---
title: Contact
icon: fas fa-envelope
order: 5
---

<!--
To make this contact form work, you need to sign up for a free account at https://formspree.io/ and replace the email address in the `action` attribute of the form with your own.
-->
<form action="https://formspree.io/f/{{ site.social.email }}" method="POST">
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" name="name" id="name" class="form-control">
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" name="_replyto" id="email" class="form-control">
  </div>
  <div class="form-group">
    <label for="message">Message</label>
    <textarea name="message" id="message" class="form-control" rows="5"></textarea>
  </div>
  <button type="submit" class="btn btn-primary">Send</button>
</form>
