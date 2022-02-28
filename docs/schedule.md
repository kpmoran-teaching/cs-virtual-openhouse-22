---
hide:
  - navigation 
  - toc        
---

## Open House Schedule

<script src="//code.iconify.design/1/1.0.6/iconify.min.js"></script>

<script src="https://momentjs.com/downloads/moment.js"></script>
<script src="https://momentjs.com/downloads/moment-timezone-with-data-10-year-range.js"></script>

<script>
// Get the timezone
// If it's already in storage, just grab from there
if (!sessionStorage.getItem('timezone')) {
  var tz = jstz.determine() || 'UTC';
  sessionStorage.setItem('timezone', tz.name());
}
var currTz = sessionStorage.getItem('timezone');

// References to DOM elements
var inputTime = document.querySelector("#input-time");
var output = document.querySelector("#local");

// When the input changes, update the local time
inputTime.addEventListener("change", function() {
  updateTime(this.value);
});

function updateTime(theTime) {
  
  // Format Moment.js expects:
  //   2015-08-12T14:30Z
  // Moment.js can help us build it.
  var date = moment().format("YYYY-MM-DD");
  var stamp = date + "T" + theTime + "Z";
    
  // Create a Moment.js object
  var momentTime = moment(stamp);
  
  // Adjust using Moment Timezone
  var tzTime = momentTime.tz(currTz);
  
  // Format the time back to normal
  var formattedTime = tzTime.format('h:mm A');
  
  output.textContent = "Time in " + currTz + ": " + formattedTime;
}

updateTime(inputTime.value);
</script>

!!! note ""
    **Important!** All times below are displayed in your local time zone. You can download a PDF version of the schedule with all times in EST [here](../images/open-house-schedule-est.pdf).

<table>
	<!--Header-->
	<tr>
		<th class="date"><h4>Date/Time (In Local Time)</h4></th>
		<th class="event"><h4>Event</h4></th>
		<th class="description"><h4>Description</h4></th>
		<th class="meeting"><h4>Meeting Space</h4></th>
	</tr>
	
	
<!--------------------------------------------------------------------------------->
	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date1"></b> -	<b id = "date2"></b>
		
		</b></td>
		<!-- Event --> <td>Welcome From Department Chair & PhD Program Overview</td>
		<!-- Description --> <td><ul><li style="font-size:13px";>Dept. Chair David Rosenblum will provide welcoming remarks to the admitted students. Then PhD Program Director Dr. Hakan Aydin will provide an overview of the GMU CS PhD program. <b> If you missed the presentation you can view it <a href="https://gmu.zoom.us/rec/share/9Ed2FWlEwtU96niSnFGFzHVNBr0QLBHJTsTgk63NfejfG2IjAUaSmlikC1nVxG7q.m2czb-dkg1o3X8Ie">here</a>.</b> The password was emailed to all accepted students.</li></td>
		<!-- Links -->		<td><li><a style="font-size:12px;" href="https://gmu.zoom.us/meeting/register/tJEscOyqrzMqGtK8OxwQLZsyaIjjUbicfIFj">Zoom Room 1 (Requires Registration)</a></li>
		
		</td>
		
<!--------------------------------------------------------------------------------->		
		
	</tr>
	
		<tr>
		<!-- Date --> 	<td><b>
		<b id = "date3"></b> -	<b id = "date4"></b>
		
		</b></td>
		<!-- Event --> <td>Social Event with Current & Prospective Students</td>
		<!-- Description --> <td><ul><li style="font-size:13px";>Meet your potential cohort mates and current Ph.D. students for some virtual fun!</li></td>
		<!-- Links -->		<td><li><a style="font-size:12px;" href="https://gmu.zoom.us/j/97354089171">Zoom Room 2 (requires password)</a></li>
		
		</td>
	</tr>		
	
<!--------------------------------------------------------------------------------->
	
		</tr>
	
		<tr>
		<!-- Date --> 	<td><b>
		<b id = "date5"></b> -	<b id = "date6"></b>
		
		</b></td>
		<!-- Event --> <td>Panel with Current Ph.D. Students</td>
		<!-- Description --> <td><ul><li style="font-size:13px";>Learn more about Graduate life at GMU from current Ph.D. students. The session will include some directed conversations as well as time for Q/A. You can download the slides <a href="../images/welcome-from-current-students.pdf">here</a>.</li></td>
		<!-- Links -->		<td><li><a style="font-size:12px;" href="https://gmu.zoom.us/j/97354089171">Zoom Room 2 (requires password)</a></li>
		
		</td>
	</tr>
<!--------------------------------------------------------------------------------->	
	
		<tr>
		<!-- Date --> 	<td><b>
		<b id = "date7"></b> -	<b id = "date8"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-greg-stein">Dr. Greg Stein</a>, <a href="../faculty-meetings/#dr-dov-gordon">Dr. Dov Gordon</a>, <a href="../faculty-meetings/#dr-antonios-anastasopoulos">Dr. Antonios Anastasopoulos</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->
	
		<tr>
		<!-- Date --> 	<td><b>
		<b id = "date11"></b> -	<b id = "date12"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-kevin-moran">Dr. Kevin Moran</a>, <a href="../faculty-meetings/#dr-greg-stein">Dr. Greg Stein</a>, <a href="../faculty-meetings/#dr-sanmay-das">Dr. Sanmay Das</a>, <a href="../faculty-meetings/#dr-bo-han">Dr. Bo Han</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>
	
	<!--------------------------------------------------------------------------------->
	
		<tr>
		<!-- Date --> 	<td><b>
		<b id = "date49"></b> -	<b id = "date50"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-daniel-menasce">Dr. Daniel Menasce</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>

	
<!-------------------------------------Break 1-------------------------------------------->
	
	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date9"></b> -	<b id = "date10"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->

<tr>
		<!-- Date --> 	<td><b>
		<b id = "date53"></b> -	<b id = "date54"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-yotam-gingold">Dr. Yotam Gingold</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			

<!--------------------------------------------------------------------------------->


	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date13"></b> -	<b id = "date14"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-greg-stein">Dr. Greg Stein</a>, <a href="../faculty-meetings/#dr-shuochao-yao">Dr. Shuochao Yao</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			

<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date15"></b> -	<b id = "date16"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-shuochao-yao">Dr. Shuochao Yao</a>, <a href="../faculty-meetings/#dr-erion-plaku">Dr. Erion Plaku</a>, <a href="../faculty-meetings/#dr-thomas-latoza">Dr. Thomas LaToza</a> </li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			

<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date17"></b> -	<b id = "date18"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-shuochao-yao">Dr. Shuochao Yao</a>, <a href="../faculty-meetings/#dr-sonqing-chen">Dr. Songqing Chen</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!------------------------------------Break 2--------------------------------------------->
	
	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date27"></b> -	<b id = "date28"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date19"></b> -	<b id = "date20"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-craig-yu">Dr. Craig Yu</a>, <a  href="../faculty-meetings/#dr-eric-osterweil">Dr. Eric Osterweil</a>, <a href="../faculty-meetings/#dr-jessica-lin">Dr. Jessica Lin</a>, <a href="../faculty-meetings/#dr-sanmay-das">Dr. Sanmay Das</a>, <a href="../faculty-meetings/#dr-amarda=shehu">Dr. Amarda Shehu</a>, <a href="../faculty-meetings/#dr-daniel-menasce">Dr. Daniel Menasce</a>, <a href="../faculty-meetings/#dr-huzefa-rangwala">Dr. Huzefa Rangwala</a>, <a href="../faculty-meetings/#dr-bo-han">Dr. Bo Han</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date21"></b> -	<b id = "date22"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-eric-osterweil">Dr. Eric Osterweil</a>, <a href="../faculty-meetings/#dr-jessica-lin">Dr. Jessica Lin</a>, <a href="../faculty-meetings/#dr-brittany-johnson">Dr. Brittany Johnson</a>, <a href="../faculty-meetings/#dr-parth-pathak">Dr. Parth Pathak</a>, <a href="../faculty-meetings/#dr-foteini-baldmitsi">Dr. Foteini Baldmitsi</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date23"></b> -	<b id = "date24"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-jessica-lin">Dr. Jessica Lin</a>, <a href="../faculty-meetings/#dr-brittany-johnson">Dr. Brittany Johnson</a>, <a href="../faculty-meetings/#dr-alex-brodsky">Dr. Alex Brodsky</a>, <a href="../faculty-meetings/#dr-foteini-baldmitsi">Dr. Foteini Baldmitsi</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date25"></b> -	<b id = "date26"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-kevin-moran">Dr. Kevin Moran</a>, <a href="../faculty-meetings/#dr-brittany-johnson">Dr. Brittany Johnson</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date55"></b> -	<b id = "date56"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-jeff-offutt">Dr. Jeff Offutt</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------Break 3------------------------------------------->

	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date29"></b> -	<b id = "date30"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date31"></b> -	<b id = "date32"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-greg-stein">Dr. Greg Stein</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>		
	
<!--------------------------------------------------------------------------------->

	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date57"></b> -	<b id = "date58"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-jyh-ming-lien">Dr. Jyh-Ming Lien</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>				
	
<!--------------------------------------Break 4------------------------------------------->

	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date33"></b> -	<b id = "date34"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->


	<tr>
		<!-- Date --> 	<td><b>
		<b id = "date35"></b> -	<b id = "date36"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-erion-plaku">Dr. Erion Plaku</a>, <a href="../faculty-meetings/#dr-sanmay-das">Dr. Sanmay Das</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>					
	
<!-------------------------------------Break 5-------------------------------------------->

	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date39"></b> -	<b id = "date40"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->

<tr>
		<!-- Date --> 	<td><b>
		<b id = "date41"></b> -	<b id = "date42"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-eric-osterweil">Dr. Eric Osterweil</a>, <a href="../faculty-meetings/#dr-daniel-menasce">Dr. Daniel Menasce</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

<tr>
		<!-- Date --> 	<td><b>
		<b id = "date51"></b> -	<b id = "date52"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-kevin-moran">Dr. Kevin Moran</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			

	
<!--------------------------------------Break 6------------------------------------------->

	<tr>
	<th style="vertical-align:middle;" ><b><b id = "date43"></b> -	<b id = "date44"></b></b></th>
								<th style="vertical-align:middle;" colspan=4><center><b>Break/Offline</b></center></th>
		</tr>

<!--------------------------------------------------------------------------------->
<tr>
		<!-- Date --> 	<td><b>
		<b id = "date45"></b> -	<b id = "date46"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-thomas-latoza">Dr. Thomas LaToza</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->

<tr>
		<!-- Date --> 	<td><b>
		<b id = "date47"></b> -	<b id = "date48"></b>
		
		</b></td>
		<!-- Event --> <td>Drop in Time with Faculty</td>
		<!-- Description --> <td><ul><li style="font-size:13px;">Faculty Available: <a href="../faculty-meetings/#dr-shuochao-yao">Dr. Shuochao Yao</a>, <a href="../faculty-meetings/#dr-jyh-ming-lien">Dr. Jyh-Ming Lien</a></li></td>
		<!-- Links -->		<td><li style="font-size:12px;">Individual Faculty Zoom Rooms</li>
		
		</td>
	</tr>			
	
<!--------------------------------------------------------------------------------->


</table>

<script>
    var a = moment("2021-03-15T13:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date1").innerHTML = a;
    
    var b = moment("2021-03-15T14:00:00.000Z").format('h:mm A')
    document.getElementById("date2").innerHTML = b;
    
    var c = moment("2021-03-15T14:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date3").innerHTML = c;
    
    var d = moment("2021-03-15T15:00:00.000Z").format('h:mm A')
    document.getElementById("date4").innerHTML = d;
    
     var e = moment("2021-03-15T15:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date5").innerHTML = e;
    
    var f = moment("2021-03-15T16:00:00.000Z").format('h:mm A')
    document.getElementById("date6").innerHTML = f;
    
    var g = moment("2021-03-15T16:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date7").innerHTML = g;
    
    var h = moment("2021-03-15T17:00:00.000Z").format('h:mm A')
    document.getElementById("date8").innerHTML = h;
    
    var i = moment("2021-03-15T19:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date9").innerHTML = i;
    
    var j = moment("2021-03-15T20:30:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date10").innerHTML = j;
    
    var k = moment("2021-03-15T17:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date11").innerHTML = k;
    
    var l = moment("2021-03-15T18:00:00.000Z").format('h:mm A')
    document.getElementById("date12").innerHTML = l;
    
    var m = moment("2021-03-15T22:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date13").innerHTML = m;
    
    var n = moment("2021-03-15T23:00:00.000Z").format('h:mm A')
    document.getElementById("date14").innerHTML = n;
    
    var o = moment("2021-03-15T23:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date15").innerHTML = o;
    
    var p = moment("2021-03-15T24:00:00.000Z").format('h:mm A')
    document.getElementById("date16").innerHTML = p;

    var q = moment("2021-03-15T24:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date17").innerHTML = q;
    
    var r = moment("2021-03-16T01:00:00.000Z").format('h:mm A')
    document.getElementById("date18").innerHTML = r;
    
    var s = moment("2021-03-16T14:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date19").innerHTML = s;
    
    var t = moment("2021-03-16T15:00:00.000Z").format('h:mm A')
    document.getElementById("date20").innerHTML = t;
    
    var u = moment("2021-03-16T15:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date21").innerHTML = u;
    
    var v = moment("2021-03-16T16:00:00.000Z").format('h:mm A')
    document.getElementById("date22").innerHTML = v;
    
    var w = moment("2021-03-16T16:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date23").innerHTML = w;
    
    var x = moment("2021-03-16T17:00:00.000Z").format('h:mm A')
    document.getElementById("date24").innerHTML = x;
    
    var y = moment("2021-03-16T17:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date25").innerHTML = y;
    
    var z = moment("2021-03-16T18:00:00.000Z").format('h:mm A')
    document.getElementById("date26").innerHTML = z;
    
    var aa = moment("2021-03-16T01:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date27").innerHTML = aa;
    
    var bb = moment("2021-03-16T14:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date28").innerHTML = bb;
    
    var cc = moment("2021-03-16T18:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date29").innerHTML = cc;
    
    var dd = moment("2021-03-16T22:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date30").innerHTML = dd;
    
    var ee = moment("2021-03-16T22:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date31").innerHTML = ee;
    
    var ff = moment("2021-03-16T23:00:00.000Z").format('h:mm A')
    document.getElementById("date32").innerHTML = ff;

    var gg = moment("2021-03-17T01:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date33").innerHTML = gg;
    
    var hh = moment("2021-03-17T14:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date34").innerHTML = hh;
    
    var ii = moment("2021-03-17T14:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date35").innerHTML = ii;
    
    var jj = moment("2021-03-17T15:00:00.000Z").format('h:mm A')
    document.getElementById("date36").innerHTML = jj;

    var ll = moment("2021-03-17T15:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date39").innerHTML = ll;
    
    var mm = moment("2021-03-17T17:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date40").innerHTML = mm;

    var nn = moment("2021-03-17T17:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date41").innerHTML = nn;
    
    var oo = moment("2021-03-17T18:00:00.000Z").format('h:mm A')
    document.getElementById("date42").innerHTML = oo;

    var pp = moment("2021-03-17T19:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date43").innerHTML = pp;
    
    var qq = moment("2021-03-17T23:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date44").innerHTML = qq;

    var rr = moment("2021-03-17T23:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date45").innerHTML = rr;
    
    var ss = moment("2021-03-17T24:00:00.000Z").format('h:mm A')
    document.getElementById("date46").innerHTML = ss;
    
    var tt = moment("2021-03-17T24:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date47").innerHTML = tt;
    
    var uu = moment("2021-03-18T01:00:00.000Z").format('h:mm A')
    document.getElementById("date48").innerHTML = uu;
    
    var vv = moment("2021-03-15T18:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date49").innerHTML = vv;
    
    var ww = moment("2021-03-15T19:00:00.000Z").format('h:mm A')
    document.getElementById("date50").innerHTML = ww;

    var xx = moment("2021-03-17T18:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date51").innerHTML = xx;
    
    var yy = moment("2021-03-17T19:00:00.000Z").format('h:mm A')
    document.getElementById("date52").innerHTML = yy;
    
    var aaa = moment("2021-03-15T20:30:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date53").innerHTML = aaa;
    
    var bbb = moment("2021-03-15T21:30:00.000Z").format('h:mm A')
    document.getElementById("date54").innerHTML = bbb;
    
    var ccc = moment("2021-03-16T18:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date55").innerHTML = ccc;
    
    var ddd = moment("2021-03-16T20:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date56").innerHTML = ddd;

    var eee = moment("2021-03-16T24:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date57").innerHTML = eee;
    
    var fff = moment("2021-03-17T01:00:00.000Z").format('MMMM D, h:mm A')
    document.getElementById("date58").innerHTML = fff;


    
</script>
