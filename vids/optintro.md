---
layout: page
title: "Optimization Introduction"
meta_title: "optintro"
permalink: "/vids/optintro/"
---


<html>
<head>
<script>

function setCookie(cname,cvalue,exdays) {
    var d = new Date();
    d.setTime(d.getTime() + (exdays*24*60*60*1000));
    var expires = "expires=" + d.toGMTString();
    document.cookie = cname + "=" + cvalue + ";" + expires + ";path=/";
}

function getCookie(cname) {
    var name = cname + "=";
    var decodedCookie = decodeURIComponent(document.cookie);
    var ca = decodedCookie.split(';');
    for(var i = 0; i < ca.length; i++) {
        var c = ca[i];
        while (c.charAt(0) == ' ') {
            c = c.substring(1);
        }
        if (c.indexOf(name) == 0) {
            return c.substring(name.length, c.length);
        }
    }
    return "";
}

function checkCookie() {
    var vidchoice=getCookie("optintro");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvidstest/in/c/optintro";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvidstest/in/o/optintro";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvidstest/in/v/optintro";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/c/optintro";}
    else if (vidchoice==5){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/o/optintro";}
    else if (vidchoice==6){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/v/optintro";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= (1/6) ){
        setCookie("optintro", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= (2/6) ){
        setCookie("optintro", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= (3/6) ){
        setCookie("optintro", 3, 365);
        checkCookie();
        }
        else if (forwardchoice <= (4/6) ){
          setCookie("optintro", 4, 365);
          checkCookie();
          }
          else if (forwardchoice <= (5/6) ){
            setCookie("optintro", 5, 365);
            checkCookie();
            }
      else {
        setCookie("optintro", 6, 365);
        checkCookie();
        }
      }
}



</script>
</head>
<body onload="checkCookie()">
Loading...
</body>
</html>
