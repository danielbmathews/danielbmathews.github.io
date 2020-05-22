
_Careers are a jungle gym, not a ladder._ -Sheryl Sandberg

<img src='https://g.gravizo.com/svg?
 digraph G {
    rankdir = BT
    communications -> coding;
    communications -> analytics;
    communications -> managing;
    coding -> ETL;
    coding -> algorithms;
    analytics -> algorithms;
    analytics -> "domain expertise";
    managing -> coaching;
    coaching -> leading;
    managing -> planning;
    "Data Engineer" [shape = box];
    "Data Scientist" [shape = box];
    "Business analyst" [shape = box];
    Manager [shape = box];
    "Program / Project Manager" [shape = box];
    ETL -> "Data Engineer";
    algorithms -> "Data Scientist";
    "domain expertise" -> "Business analyst";
    leading -> Manager;
    planning -> "Program / Project Manager";
 }
'/>