---
layout: post
title: My Second Post
---
<div class="container">
It's final time, here be a simple attempt at utalizing a .js script and flex box

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/typed.js/2.0.12/typed.min.js"></script>
<script>
  $(function() {
    var typed = new Typed('.typed', {
      strings: ['My homebuying process'],
      typeSpeed: 50,
      backSpeed: 50,
      loop: true
    });
  });
</script>
<h2 class="typed"></h2>
I guess I could talk about my homebuying process. It has been going well, I'm rather young to be buying a house, but my wife and I found a good starter home in Columbia, PA.
 I'm glad I left Oregon last year, I could've never bought a house there.
 
  <label for="Comment">Comment?:</label>
  <input type="text" id="Comment"><br><br>
  <button onclick="openDialog()">Submit</button>
 <script>
  function openDialog() {
    document.getElementById("Thanks").showModal();
  }
  function closeDialog() {
    document.getElementById("Thanks").close();
  }
</script>
<dialog id="Thanks">
  <h2>Thanks</h2>
  <p>Your comment is appreciated.</p>
  <button onclick="closeDialog()">Close Dialog</button>
</dialog>
<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .posts-container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .post {
    margin: 25px;
    padding: 25px;
    border: 3px solid black;
    width: 80%;
    max-width: 800px;
  }