# Room 1: the RSE office

![A picture of the office](assets/rse-office.jpg)

You arrive at the RSE office a few minutes early, only to find it completely deserted. The team must be out at a meeting, and surely they'll be back soon.

There's a couple of cheap but comfy-looking chairs next to a coatstand near the door, so assuming these are intended for guests you take a seat. This office is in a newer part of the campus, on the other side from your department's main building, so you've had a few minutes' walk to get there.

While you wait you cast your eye around the room: maybe you can figure out what an RSE does by studying their natural environment! Next to your seat there is a desk, obviously well used by its usual occupant.

- There is a *cup of coffee* on the desk. It's still steaming, so its owner can't be far away.
- There is an *open laptop* on the desk, with a *newspaper* right next to it. The laptop screen is on, but locked, and a password prompt is showing.
- There is a *bookshelf* with a few books on it. You scan your eyes over the titles on the spines hoping for some insight. For some reason a lot of them are about snakes? Maybe RSEs mostly work with zoologists...

## Actions:
<details><summary>Look at the cup of coffee</summary>
<p>
The coffee is still warm. There is something written on the bottom of the cup: "Passcode is the number of letters in API"
</p>
</details>
<details><summary>Look at the newspaper</summary>
<p>
It's from last week. Someone has already filled in the crossword
</p>
</details>
<details><summary>Look at the bookshelf</summary>
<ul>
  <li>The novel is "The Left Hand of Darkness" by Ursula Le Guin. it's old and worn. It looks like a fun read, but you don't have time for this at the moment.</li>
  <li>"Design Patterns: Elements of Reusable Object Oriented Software". it looks like the cover was originally white, but as now turned gray. Most of the pages contain scribbled drawings.</li>
  <li>"Web APIs for the 20th century": This looks interesting... Maybe I should look at this in more detail.</li>
</ul> 
</details>

<details><summary>Look at "Web APIs for the 20th century"</summary>
<p>
You have a sift through this book, there is a lot of jargon that you don't understand. However you do see that on the first page it mentions something called a Application Programming Interface, "In building applications, an API (application programming interface) simplifies programming by abstracting the underlying implementation and only exposing objects or actions the developer needs.".
</p>
</details>

## Enter passcode to computer:

<input type="text" id="puzzle-1" name="name"/>
<input type="button" value="click" onclick="check()">
<br/>

<span id="err"></span>

<script>
function check()
{
  var a=document.getElementById("puzzle-1");
  if((a.value=="31"))
  {
    document.getElementById('err').innerHTML= 'Correct, now let us have a look at the <a href="/ah-software-escape-room/laptop.html">laptop</a>';
  }
  else if(a.value=="3") 
  {
    document.getElementById('err').innerHTML= 'Not quite! Try again';
  }
  else if(a.value=="33") 
  {
    document.getElementById('err').innerHTML= 'Try it without spaces!';

  }
  else
  {
    document.getElementById('err').innerHTML= 'Incorrect passcode';
  }
}
</script>
