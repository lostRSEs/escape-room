## Intro
You are a researcher in the classics department. You have been told you need to meet an "RSE", whatever that is. You are given a name and address to go to. When you arrive at the office you find it completely empty...

### Room 1: the RSE office
It is empty of people. There is a *cup of coffee* on the desk. There is an *open laptop* on the desk, with a *newspaper* right next to it. There is a *bookshelf* with a few books on it. 

#### Visible items:
 - Cup of coffee
 - An open laptop which is locked and asking for a passcode
 - A newspaper
 - Bookshelf has books: 
   - "Design Patterns: Elements of Reusable Object Oriented Software"
   - A novel: "The Left Hand of Darkness" by Ursula Le Guin
   - A book: Web APIs for the 20th century

#### Actions:
<details><summary>Look on the underside of the coffee mug</summary>
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

  - novel: it's old and worn. It looks like a fun read, but you don't have time for this at the moment.
  - "Design Patterns: Elements of Reusable Object Oriented Software". it looks like the cover was originally white, but as now turned gray. Most of the pages contain scribbled drawings.
  - "Web APIs for the 20th century": This looks interesting...

</details>

<details><summary>Look at "Web APIs for the 20th century"</summary>
<p>
You have a sift through this book, there is a lot of jargon that you don't understand. However you do see that on the first page it mentions something called a Application Programming Interface, "In building applications, an API (application programming interface) simplifies programming by abstracting the underlying implementation and only exposing objects or actions the developer needs.".
</p>
</details>

#### Enter passcode to computer:

<input type="text" id="puzzle-1" name="name"/>
<input type="button" value="click" onclick="check()"><span id="err"></span>

<script>
function check()
{
  var a=document.getElementById("puzzle-1");
  if((a.value=="31"))
  {
    document.getElementById('err').innerHTML= 'correct go to the <a href="/page2">next</a> page';
  }
  else
  {
    document.getElementById('err').innerHTML= 'wrong';
  }
}
</script>
