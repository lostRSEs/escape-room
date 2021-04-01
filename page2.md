# Page 2
Open on the laptop, there is a web browser open with a number of tabs.

## Actions:
<details><summary>Look at browser tab 1</summary>
<p>
Going through the browser tabs, you see another web page open which is entitled "Web API for RSE locations".
</p>

<p>
It lists the following:
</p>
<ul>
<li>GET /list                 Lists the IDs for all of the RSEs</li>
<li>GET /location/$id         Get the location of a single RSE</li>
<li>GET /calendar/$id         Get the calendar for a particular RSE</li>
<li>GET /conference/$conf-id  Get the calendar for a particular RSE</li>
</ul>
</details>

<details><summary>Look at browser tab 2</summary>
This is is some text and a text box asking "I ma erehW?".
</details>

<details><summary>Look at Terminal</summary>
You see there is a Terminal window open with the command:


    $ curl https://rse-api.my-university.com/rse-api/list
    ["RSE-002", "RSE-443", "321-ESR"]
    $ 
</details>

## Execute location query

curl https://rse-api.my-university.com/rse-api/location/<input type="text" id="location-text" name="name"/>
<input type="button" value="click" onclick="check()">
<br/>

<span id="location"></span>

<script>
function check()
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
At conference: CONF-003
  }
  else
  {
    document.getElementById('location').innerHTML= '404, not found';
  }
}
</script>

## Execute conference query

curl https://rse-api.my-university.com/rse-api/conference/<input type="text" id="conference-text" name="name"/>
<input type="button" value="click" onclick="check()">
<br/>

<span id="conference"></span>

<script>
function check()
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
