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
<input type="text" id="puzzle-1" name="name"/>
<input type="button" value="click" onclick="check()"><span id="err"></span>

<script>
function check()
{
  var a=document.getElementById("puzzle-1");
  if((a.value=="31"))
  {
    document.getElementById('err').innerHTML= 'correct';
  }
  else
  {
    document.getElementById('err').innerHTML= 'wrong';
  }
}
</script>
