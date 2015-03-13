---
title: "Forms(dev)"
description: ""
---

<div class="Container">


<h1>Forms</h1>

<form>
  <fieldset>
    <legend>Inputs as descendents of labels (form legend). This doubles up as a long legend that can test word wrapping.</legend>
    <p><label>Text input <input type="text" value="default value that goes on and on without stopping or punctuation"></label></p>
    <p><label>Email input <input type="email"></label></p>
    <p><label>Search input <input type="search"></label></p>
    <p><label>Tel input <input type="tel"></label></p>
    <p><label>URL input <input type="url" placeholder="http://"></label></p>
    <p><label>Password input <input type="password" value="password"></label></p>
    <p><label>File input <input type="file"></label></p>

    <p><label>Radio input <input type="radio" name="rad"></label></p>
    <p><label>Checkbox input <input type="checkbox"></label></p>
    <p><label><input type="radio" name="rad"> Radio input</label></p>
    <p><label><input type="checkbox"> Checkbox input</label></p>

    <p><label>Select field <select><option>Option 01</option><option>Option 02</option></select></label></p>
    <p><label>Textarea <textarea cols="30" rows="5" >Textarea text</textarea></label></p>
  </fieldset>

  <fieldset>
    <legend>Inputs as siblings of labels</legend>
    <p><label for="ic">Color input</label> <input type="color" id="ic" value="#000000"></p>
    <p><label for="in">Number input</label> <input type="number" id="in" min="0" max="10" value="5"></p>
    <p><label for="ir">Range input</label> <input type="range" id="ir" value="10"></p>
    <p><label for="idd">Date input</label> <input type="date" id="idd" value="1970-01-01"></p>
    <p><label for="idm">Month input</label> <input type="month" id="idm" value="1970-01"></p>
    <p><label for="idw">Week input</label> <input type="week" id="idw" value="1970-W01"></p>
    <p><label for="idt">Datetime input</label> <input type="datetime" id="idt" value="1970-01-01T00:00:00Z"></p>
    <p><label for="idtl">Datetime-local input</label> <input type="datetime-local" id="idtl" value="1970-01-01T00:00"></p>

    <p><label for="irb">Radio input</label> <input type="radio" id="irb" name="rad"></p>
    <p><label for="icb">Checkbox input</label> <input type="checkbox" id="icb"></p>
    <p><input type="radio" id="irb2" name="rad"> <label for="irb2">Radio input</label></p>
    <p><input type="checkbox" id="icb2"> <label for="icb2">Checkbox input</label></p>

    <p><label for="s">Select field</label> <select id="s"><option>Option 01</option><option>Option 02</option></select></p>
    <p><label for="t">Textarea</label> <textarea id="t" cols="30" rows="5" >Textarea text</textarea></p>
  </fieldset>

  <fieldset>
    <legend>Clickable inputs and buttons</legend>
    <p><input type="image" src="http://lorempixel.com/90/24" alt="Image (input)"></p>
    <p><input type="reset" value="Reset (input)"></p>
    <p><input type="button" value="Button (input)"></p>
    <p><input type="submit" value="Submit (input)"></p>
    <p><input type="submit" value="Disabled (input)" disabled></p>

    <p><button type="reset">Reset (button)</button></p>
    <p><button type="button">Button (button)</button></p>
    <p><button type="submit">Submit (button)</button></p>
    <p><button type="submit" disabled>Disabled (button)</button></p>
  </fieldset>

  <fieldset id="boxsize">
    <legend>box-sizing tests</legend>
    <div><input type="text" value="text"></div>
    <div><input type="email" value="email"></div>
    <div><input type="search" value="search"></div>
    <div><input type="url" value="http://example.com"></div>
    <div><input type="password" value="password"></div>

    <div><input type="color" value="#000000"></div>
    <div><input type="number" value="5"></div>
    <div><input type="range" value="10"></div>
    <div><input type="date" value="1970-01-01"></div>
    <div><input type="month" value="1970-01"></div>
    <div><input type="week" value="1970-W01"></div>
    <div><input type="datetime" value="1970-01-01T00:00:00Z"></div>
    <div><input type="datetime-local" value="1970-01-01T00:00"></div>

    <div><input type="radio"></div>
    <div><input type="checkbox"></div>

    <div><select><option>Option 01</option><option>Option 02</option></select></div>
    <div><textarea cols="30" rows="5">Textarea text</textarea></div>

    <div><input type="image" src="http://lorempixel.com/90/24" alt="Image (input)"></div>
    <div><input type="reset" value="Reset (input)"></div>
    <div><input type="button" value="Button (input)"></div>
    <div><input type="submit" value="Submit (input)"></div>

    <div><button type="reset">Reset (button)</button></div>
    <div><button type="button">Button (button)</button></div>
    <div><button type="submit">Submit (button)</button></div>
  </fieldset>
</form>

</div>