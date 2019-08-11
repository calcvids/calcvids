---
layout: page
title: "Definite Integrals"
meta_title: "defint"
permalink: "/vids/defint/"
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
    var vidchoice=getCookie("defint");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvidstest/in/c/defint";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvidstest/in/o/defint";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvidstest/in/v/defint";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/c/defint";}
    else if (vidchoice==5){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/o/defint";}
    else if (vidchoice==6){window.location.href = "https://ximera.osu.edu/calcvidstest/nin/v/defint";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= (1/6) ){
        setCookie("defint", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= (2/6) ){
        setCookie("defint", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= (3/6) ){
        setCookie("defint", 3, 365);
        checkCookie();
        }
        else if (forwardchoice <= (4/6) ){
          setCookie("defint", 4, 365);
          checkCookie();
          }
          else if (forwardchoice <= (5/6) ){
            setCookie("defint", 5, 365);
            checkCookie();
            }
      else {
        setCookie("defint", 6, 365);
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
