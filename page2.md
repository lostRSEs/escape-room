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

 - curl https://rse-api.my-university.com/rse-api/location/RSE-002    : This prints out: "At home"
 - curl https://rse-api.my-university.com/rse-api/location/RSE-443    : This prints out: "At conference: CONF-003"
 - curl https://rse-api.my-university.com/rse-api/location/RSE-231    : This prints out: "At conference: CONF-003"
 - curl https://rse-api.my-university.com/rse-api/conference/CONF-003 : This prints out: "At Collaborations workshop 2021 (CW21)"


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
