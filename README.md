<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<HTML><HEAD><TITLE> Quiz Aritmetico</TITLE>
<META http-equiv=Content-Type content="text/html; charset=iso-8859-1">
<js/StyleDemo.css" type=text/css rel=stylesheet>
<SCRIPT language=JavaScript>




<!-- Begin
correct=0;
wrong=0;

function random(maxValue) {
day= new Date();
hour= day.getHours();
min=day.getMinutes();
sec=day.getSeconds();
mili=day.getTime()
return(((hour*3600)+(min*60)+(sec)+mili) % maxValue);
}
function ranom(maxValue) {
day= new Date();
mil=day.getTime();
return((mil) % maxValue);
}

function add() {
if(document.quizform.arithmetic[0].checked)
maxValue=10;
else {
if(document.quizform.arithmetic[1].checked)
maxValue=30;
else {
maxValue=60;
   }
}
numA=random(maxValue);
numB=ranom(maxValue);
numC=numA + numB;
Answer=window.prompt(  numA + "+"  + numB +  " = ", "");
ans();
}
function subtract() {
if(document.quizform.arithmetic[0].checked)
maxValue=10;
else
{if(document.quizform.arithmetic[1].checked)
maxValue=30;
else {
maxValue=60
   }
}
numA=random(maxValue);
numB=ranom(maxValue);
numC=numA - numB;
Answer=window.prompt(  numA + "-"  + numB+  " = ", 0);
ans()
}
function divide() {
if(document.quizform.arithmetic[0].checked)
maxValue=10;
else {
if(document.quizform.arithmetic[1].checked)
maxValue=30;
else {
maxValue=60
   }
}
numA=random(maxValue)+1;
numB=ranom(maxValue)+1;
numC=numA / numB;
numC=Math.round(numC)
window.alert("Please round your answer off:\n"
+".5 or higher rounds one number up\n"
+".4 or lower rounds one number down");
Answer=window.prompt(  numA + "/"  + numB +  " = ", 0);
ans()
}
function multiply() {
if(document.quizform.arithmetic[0].checked)
maxValue=10;
else {
if(document.quizform.arithmetic[1].checked)
maxValue=30;
else {
maxValue=60
   }
}
numA=random(maxValue);
numB=ranom(maxValue);
numC=numA * numB;
Answer=window.prompt(  numA + "*"  + numB +  " = ", 0);
ans();
}
function check() {
if ((correct+wrong) != 0) {
score = "" + ((correct / (correct + wrong)) * 100);
score = score.substring(0,4) + "%";
alert("YOUR SCORE:  " + score + "\n" 
+ correct + " correct\n"
+ wrong + " incorrect")
}
else alert("Non hai finito tutti gli esercizi.");
}
function ans() {
if (Answer == numC) {
correct++;
msg = "Congratulazioni, il risultato è corretto!";
}
else {
wrong++;
msg = "Oops!  " + Answer + " is incorrect.\n\n"
+ "The correct answer was " +numC + ".";
   }
score = "" + ((correct / (correct + wrong)) * 100);
score = score.substring(0,4) + "%";
alert(msg + "\n\nPunteggio:  " + score + "\n" 
+ correct + " correct\n"
+ wrong + " incorrect")
}
//  End -->
</SCRIPT>

<META content="MSHTML 6.00.6000.16525" name=GENERATOR></HEAD>
<BODY>

     
    <TD 
  
<TABLE cellSpacing=0 cellPadding=0 width="100%" border=0>
  <TBODY>
  <TR>
    <TD width=24>&nbsp;</TD>
    <TD>
      <SCRIPT language=JavaScript 
      
      type=text/javascript></SCRIPT>
    </TD></TR></TBODY></TABLE>

<DIV align=center><font face="verdana"><font size="5">
QUIZ ARITMETICO</font><br><br><br>
<font size="2">



<FORM name=quizform><INPUT class=button onclick=add() type=button value=Addiziona> <INPUT class=button onclick=subtract() type=button value=Sottrai> <INPUT class=button onclick=multiply() type=button value=Moltiplica> <INPUT class=button onclick=divide() type=button value=Dividi> <BR><BR><INPUT 
type=radio name=arithmetic>Facile <INPUT type=radio CHECKED 
name=arithmetic>Medio <INPUT type=radio name=arithmetic>Difficile <BR><BR><INPUT class=button onclick=check() type=button value="Punteggio"> <INPUT class=button onclick=javascript:correct=0;wrong=0; type=button value="Azzera tutto"> 
</FORM></DIV></BODY></HTML>
<p align="center"><font size="2">
<br><br>
<a href="Menu per i giochi.htm">Torna al menu dei giochi</a><br><br>
<a href="index.htm">Home Page</a>
