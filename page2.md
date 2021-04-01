# Page 2
Open on the laptop, there is a web browser open with a number of tabs.

## Actions:
<a href="https://github.com/lostRSEs/wherearemycolleagues">Look at browser tab 1</a>

<details><summary>Look at browser tab 2</summary>
This is is some text and a text box asking "I ma erehW?".
</details>

<details><summary>Look at Terminal</summary>
You see there is a Terminal window open with the command:


<pre><code>
    $ curl https://rse-api.my-university.com/rse-api/list
    ["RSE-002", "RSE-443", "321-ESR"]
    $ 
</code></pre>
</details>

## Execute list query

curl https://rse-api.my-university.com/rse-api/list
<input type="button" value="click" onclick="list()">
<br/>

<span id="list-span"></span>

<script>
function list()
{
  var a=document.getElementById("list-span");
  document.getElementById('list-span').innerHTML= '200, ["RSE-002", "RSE-443", "321-ESR"]';
}
</script>

## Execute location query

curl https://rse-api.my-university.com/rse-api/location/<input type="text" id="location-text" name="name"/>
<input type="button" value="click" onclick="locationCheck()">
<br/>

<span id="location"></span>

<script>
function locationCheck()
{
  var a=document.getElementById("location-text");
  if((a.value.toLowerCase()=="rse-002"))
  {
    document.getElementById('location').innerHTML= '200, At home';
  }
  else if((a.value.toLowerCase()=="rse-443"))
  {
    document.getElementById('location').innerHTML= '200, In maths department';
  }
  else if((a.value.toLowerCase()=="321-esr"))
  }
  else
  {
    document.getElementById('location').innerHTML= '404, not found';
  }
}
</script>

## Execute conference query

curl https://rse-api.my-university.com/rse-api/conference/<input type="text" id="conference-text" name="name"/>
<input type="button" value="click" onclick="conferenceCheck()">
<br/>

<span id="conference"></span>

<script>
function conferenceCheck()
{
  var a=document.getElementById("conference-text");
  if((a.value.toLowerCase()=="conf-003"))
  {
    document.getElementById('conference').innerHTML= '200, At Collaborations workshop 2021 (CW21)';
  }
  else
  {
    document.getElementById('conference').innerHTML= '404, not found';
  }
}
</script>

## I ma erehW?

<input type="text" id="puzzle-1" name="name"/>
<input type="button" value="click" onclick="check()">
<br/>

<span id="err"></span>

<script>
function check()
{
  var a=document.getElementById("puzzle-1");
  if((a.value.toLowerCase()=="cw21")|| (a.value.toLowerCase()=="collaborations workshop 2021")
  {
    document.getElementById('err').innerHTML= 'Correct go to the <a href="/ah-software-escape-room/page3">next</a> page';
  }
  else
  {
    document.getElementById('err').innerHTML= 'Inorrect';
  }
}
</script>
