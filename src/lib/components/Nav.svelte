<!-- mobile navbar -->

  <input type="checkbox" name="hamburger" id="hamburger">
  <label for="hamburger">♡</label>
<nav class="nav-mobile">
    <ul>
       <h1>Nandita Badeloe</h1>
       <li><a href="/">Home</a></li>
      <li><a href="/">Design</a></li>
      <li><a href="/">Projects</a></li>
      <li><a href="/">Contact</a></li>
    </ul>
</nav>
<!-- desptop navbar -->
<nav class="nav-desktop">
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/">Design</a></li>
    <h1>Nandita Badeloe</h1>
    <li><a href="/">Projects</a></li>
    <li><a href="/">Contact</a></li>
  </ul>
</nav>

<style>
    .nav-mobile{
        display: none;
    }
    input, label{
        display: none;
    }
  .nav-desktop {
    background-color: aqua;
    color: #f9f9f9;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 4em;
    width: 90%;
    margin: auto;
    border-radius: 2em;
    border: 2px #f9f9f9 solid;
  }
  .nav-desktop  > ul {
    display: flex;
    justify-content: space-between;
  }

  .nav-desktop  > ul,
  li {
    list-style: none;
    padding: 1em;
    margin: 1em 4em;
  }

  .nav-desktop  > ul a {
    color: #f9f9f9;
    text-decoration: none;
  }
  @media screen and (min-width: 390px) and (max-width: 950px) {
    .nav-desktop  {
      background-color: pink;
      height: 3.5em;
      flex-direction: column;
    }
    .nav-desktop  > ul,
    li {
      list-style: none;
      padding: 0.5em;
      margin: 1.5em 2em;
      align-items: center;
    }
    ul > h1 {
      margin: 0 1em;
    }
  }

/* styling navbar mobile */

  @media screen and (min-width: 0px) and (max-width: 650px) {
      .nav-desktop {
        display: none;
    }
    #hamburger{
        display: none;
    }
    #hamburger:checked ~ .nav-mobile{
        display: flex;
        align-items: center;
        background-color: darkseagreen;
        height: fit-content;
        width: 90%;
   }
   label{
    text-align: left;
    display: block;
    padding: 0.5em;
    line-height: 1.6em;
    align-self: center;
   }
   
     
    .nav-mobile > ul,
    li {
        display: flex;
        flex-direction: column;
      list-style: none;
      align-items: center;
    }
    
    input[type="checkbox"]{
        background-color: aqua;
    }
  
  }
</style>
