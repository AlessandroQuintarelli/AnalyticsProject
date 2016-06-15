<link rel="stylesheet" href="http://netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap.min.css">
<style type="text/css"> body {padding: 10px 30px 10px 30px;} table,th, td {text-align: center;} </style>


Financial Data Segmentation: Factor Analysis
========================================================

**Arina Bobrova, Dennis Maroulis, Tavleen Kaur, Ville Herlin**


Business Decisions
---------------------------------------------------------
Analyze the correlation between different companies in the Vietnamise stock market.


The Data
--------------------------------------------------------------

We analyze 900 companies based on 17 different variables including market cap, EBITDA, PE, e.t.c. listed in the vietnamise stock market



This is how the first 50 data looks:
<br>

<div class="row">
<div class="col-md-40">
<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID2704c4757d2 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "1",
109961979.3,
8.33,
0.89,
6.66,
5.33,
10.05,
0.4,
155608084.6,
1.71,
1.34,
1.48,
144807475.6,
0.08,
32442631.15,
14604143.61,
-4735726.09,
10913214.64 
],
[
 "2",
2105263.16,
0,
0,
0,
0,
0,
0.14,
2309577.34,
11.28,
0,
0,
1598308.89,
0,
4440875.11,
0,
0,
0 
],
[
 "3",
77548764.65,
46.77,
1.85,
9.24,
0.51,
18.46,
0.67,
225969361,
0.7,
0.49,
1.01,
316874249.8,
0,
436280188.8,
1237523.32,
-1047873.2,
4124908.17 
],
[
 "4",
1146367.26,
11.98,
0.58,
0,
0,
0,
0.47,
2045157.31,
0.71,
0.71,
1.05,
3640655.58,
0.05,
2374242.79,
69677.54,
-292561.5,
0 
],
[
 "5",
1056211.96,
11.74,
1.58,
8.45,
0.59,
0,
0.82,
4495701.97,
0.44,
0.67,
1.04,
13355537.2,
0,
7420672.13,
48852.36,
-1415.4,
-88180.83 
],
[
 "6",
9204362.35,
3.7,
2.11,
10.26,
0.65,
2.68,
0.67,
34006365.07,
0.66,
0.7,
1.04,
63182552.94,
0.06,
57906321.65,
1664586.01,
-1553394.77,
1169811.85 
],
[
 "7",
3458900.89,
6.45,
0,
4.91,
1.51,
9.1,
0,
3392214.51,
1.39,
1.85,
4.09,
2971825.89,
0.05,
2178438.25,
485720.59,
-311962.39,
376187.44 
],
[
 "8",
5104672.4,
8.08,
0,
9.09,
2.26,
18.21,
0.11,
4309143.71,
1.51,
2.74,
2.75,
3560337.63,
0.08,
1836794,
608847.12,
-26843.42,
38174.47 
],
[
 "9",
1933404.94,
7.7,
0.13,
4.61,
0.54,
4.99,
0.13,
2097593.22,
0.47,
2.46,
2.7,
4596363.06,
0,
3867553.48,
312135.26,
-67452.4,
378384.94 
],
[
 "10",
2604189.04,
0,
0,
0,
0,
0,
0.23,
1745606.99,
0.63,
0,
0,
6633387.89,
0.1,
12787352.12,
0,
-286885.01,
293885.42 
],
[
 "11",
47902255.64,
9.3,
0.11,
0,
0,
0,
0.01,
40575252.15,
0.41,
1.7,
1.74,
7312629.21,
0,
14609392.62,
172228.01,
-1123891.86,
0 
],
[
 "12",
7561314,
0,
0,
0,
0,
0,
0,
3294702.8,
1.01,
0,
0,
11083042.57,
0.06,
22922933.64,
0,
-1283163.58,
0 
],
[
 "13",
1586466.17,
0,
0.18,
0,
0,
0,
0.76,
675165.35,
0.55,
1.64,
1.77,
5810657.61,
0.09,
12608057.96,
575345.08,
-1953026.98,
0 
],
[
 "14",
2404702.79,
52.36,
1.04,
6.38,
0.49,
51.2,
0.63,
5504799.44,
7.11,
0.79,
1.2,
11297312.39,
0.08,
11150995.28,
46682.23,
-105274.18,
-159729.91 
],
[
 "15",
27747941.28,
7.01,
2.04,
8.89,
1.91,
7.06,
0.78,
130628622.9,
0.56,
0.39,
1.42,
327145577.5,
0.16,
69465699.25,
4850292.47,
-846025.98,
4073395.47 
],
[
 "16",
40279269.47,
2.12,
1.18,
0,
2.87,
1.34,
0.53,
122335752.5,
0.67,
0.92,
1,
307834052.1,
0,
41357326.88,
30301922.58,
-1367218.47,
28180548.13 
],
[
 "17",
313587.49,
0,
0,
0,
0,
0,
0.99,
23442244.9,
0,
0,
0,
19972992.26,
0,
8205912.18,
0,
-425921.69,
0 
],
[
 "18",
1004097.35,
6.79,
0.08,
0,
0,
0,
0.07,
1498146.48,
1.12,
0.65,
1.3,
3286321.7,
0.1,
7524470.95,
154736.91,
-4817.34,
0 
],
[
 "19",
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0,
0 
],
[
 "20",
13956766.92,
7.43,
0,
3.69,
0.13,
11.18,
0,
6735465.86,
1.72,
3.18,
3.25,
17314955.5,
0.03,
55751141.41,
1550581.75,
-130657.03,
908369.08 
],
[
 "21",
4573755.82,
32.43,
0.51,
83.01,
15.06,
262.22,
0.62,
11310049.49,
0.32,
0.06,
0.06,
39528859.39,
0,
1143291.33,
120831.29,
-177702.75,
17369.83 
],
[
 "22",
9666851.77,
16,
4.01,
7.73,
0.77,
30.65,
0.89,
58195911.29,
0.59,
0.19,
1.01,
109885641.8,
0.06,
76680331.78,
367831.75,
-6351512.14,
312736.11 
],
[
 "23",
9720730.4,
0,
0.43,
0,
7.54,
0,
0.46,
29845013.47,
0.32,
2.36,
2.43,
58353433.05,
0,
4273881.59,
-5623883.93,
-109707.06,
-5695210.71 
],
[
 "24",
2363050.48,
4.54,
0,
-3.49,
-0.4,
6.97,
0,
-1177262.16,
1.11,
0.9,
0.98,
7556028.68,
0.14,
3040522.29,
323337.52,
-69454.75,
340542.84 
],
[
 "25",
1068194.87,
0,
0,
0,
0,
0,
0,
1069343.47,
0,
0,
0,
154750385.1,
0,
1231966.73,
0,
0,
0 
],
[
 "26",
18750000,
0,
0,
0,
0,
0,
0.01,
11666874.4,
2,
0,
0,
10060394.2,
0.06,
20732598.43,
0,
-183278.38,
0 
],
[
 "27",
12263829.22,
12.11,
0.19,
9.51,
0.74,
15.37,
0.35,
18575463.16,
0.38,
2.95,
3.2,
51558131.05,
0,
26801433.71,
869982.77,
-568166.41,
804532.5 
],
[
 "28",
1229860.37,
5.29,
0,
0,
0,
0,
0,
237002.91,
1.24,
3.79,
3.91,
1414160.79,
0.13,
2156423.02,
230787.96,
0,
0 
],
[
 "29",
317712.14,
0,
0,
0,
0,
0,
1.2,
2463072.27,
0.22,
0,
0,
4554125.38,
0,
829776.93,
0,
-2606.76,
0 
],
[
 "30",
707212.23,
15.99,
0.02,
8.01,
0.13,
14.94,
0.08,
641324.76,
0.63,
1.07,
1.26,
3991174.7,
0.06,
4458032.77,
44450.17,
-44035.43,
48565.98 
],
[
 "31",
1087540.28,
46.76,
2.36,
0,
1.1,
0,
0.83,
5672210.96,
0.62,
0.96,
1.56,
9595981.71,
0,
5394742.13,
50519.03,
-204137.49,
-42277.01 
],
[
 "32",
5985825.97,
61.9,
0.01,
50.41,
1.17,
53.89,
0.03,
6073473.6,
0.45,
1.32,
1.61,
15713929.7,
0,
3532710.75,
73900.64,
0,
92832.94 
],
[
 "33",
29900644.47,
52.05,
0,
98.19,
21.71,
60.94,
0,
30366759.79,
2.54,
1.19,
1.19,
8617463.54,
0,
3325749.37,
319538.85,
0,
299865.44 
],
[
 "34",
2909058.36,
9.22,
1.3,
22.25,
0.46,
10.32,
0.82,
11487572.22,
0.38,
0.95,
1.35,
27753691.09,
0.09,
27993504.18,
373037.73,
-6005.34,
274391.88 
],
[
 "35",
66949.93,
0.42,
0.1,
0,
0,
0,
0,
-144457.48,
0.03,
0.96,
1.18,
3378180.87,
3.25,
3086894.14,
789400.58,
-172721.98,
0 
],
[
 "36",
26442250.44,
11.3,
0.09,
4.35,
3.53,
13.2,
0.11,
28770267.21,
0.87,
0.78,
0.79,
64793466.63,
0.1,
8671075.62,
2302925.68,
-89554.27,
1982309.12 
],
[
 "37",
17974012.44,
5.74,
0.03,
3.48,
2.29,
5.74,
0.02,
8026428.19,
2.66,
9.32,
11.15,
22428889.68,
0.07,
2835045.37,
2138452.53,
-481987.36,
1643493.31 
],
[
 "38",
433225.92,
0,
0,
0,
0,
0,
0.61,
898677.5,
0.4,
0,
0,
2189128.21,
0.14,
3302860.39,
0,
-71174.38,
0 
],
[
 "39",
6623702.11,
2.79,
0.35,
2.01,
0.24,
3.31,
0.24,
4561748.46,
2.47,
0.48,
0.9,
12064732.21,
0,
13663466.07,
1498292.17,
-134336.23,
2064110.92 
],
[
 "40",
2148227.71,
36.8,
0.31,
7.51,
0.21,
34.61,
0.44,
3428769.26,
0.36,
0.6,
0.94,
16969716.51,
0,
15537058.11,
58015.13,
-46078.17,
61893.08 
],
[
 "41",
37056928.03,
6,
0.55,
5.04,
0.64,
7.27,
0.39,
54578463.25,
1.08,
0.87,
1.14,
78488936.23,
0.11,
77626556.11,
4880638.74,
-3916613.68,
1964626.1 
],
[
 "42",
34386971.21,
0,
1.38,
13.1,
0.83,
0,
0.62,
75919512.61,
0.94,
0.16,
0.97,
107299096.3,
0,
82429941,
-2817496.61,
-142484.12,
-2489794.58 
],
[
 "43",
87715.57,
0,
0,
0,
0,
0,
0,
-513862.85,
0.09,
0,
0,
1526093.81,
1.19,
4805726.42,
0,
0,
0 
],
[
 "44",
5272108.84,
0,
0,
0,
0,
0,
0.02,
4599300.75,
0.91,
0,
0,
9182086.84,
0.05,
18784715.27,
0,
-1109614.91,
0 
],
[
 "45",
24978921.07,
9.76,
0.72,
8.55,
2.27,
11.43,
0.36,
34104983.38,
1.71,
0.9,
0.91,
28637018.49,
0.04,
14342802.42,
2267726.9,
-8206842.82,
2202223.48 
],
[
 "46",
580021.48,
0,
0,
0,
0,
0,
0,
564853.81,
0,
0,
0,
1624034.72,
0.09,
1020647.17,
0,
-33659.76,
0 
],
[
 "47",
1938970.83,
0,
1.17,
8.48,
0.52,
9.14,
0.63,
5087137.69,
0.69,
1.05,
1.21,
7842900.74,
0.11,
9184468.17,
259644.36,
-211923,
218956.85 
],
[
 "48",
7921589.69,
4.72,
1.45,
7.61,
0.6,
5.49,
0.78,
25374638.98,
0.52,
0.82,
1.04,
55316039.39,
0.18,
50690227.48,
1582392.19,
-1083231.74,
1447407.94 
],
[
 "49",
2119110.59,
0,
0,
0,
0,
0,
1.13,
7423209.46,
0.53,
0,
0,
16292991.5,
0.07,
30627940.3,
0,
-40726.24,
0 
],
[
 "50",
45912833.78,
6.66,
0,
4.77,
1.71,
7.95,
0,
41006747.76,
3.16,
1.9,
3.15,
17789459.36,
0.04,
22591604.96,
5491370.81,
-388267.82,
5722625.26 
] 
];
data.addColumn('string','Variables');
data.addColumn('number','Company.Market.Cap..USD.');
data.addColumn('number','Historic.P.E..FY0.');
data.addColumn('number','Total.Debt.to.Total.Equity..Percent..FY0.');
data.addColumn('number','Enterprise.Value.To.EBITDA..Daily.Time.Series.Ratio.');
data.addColumn('number','Enterprise.Value.To.Sales..Daily.Time.Series.Ratio.');
data.addColumn('number','P.E..Daily.Time.Series.Ratio.');
data.addColumn('number','Total.Debt.To.Enterprise.Value..Daily.Time.Series.Ratio.');
data.addColumn('number','Enterprise.Value..Daily.Time.Series...USD.');
data.addColumn('number','Price.To.Book.Value.Per.Share..Daily.Time.Series.Ratio.');
data.addColumn('number','Quick.Ratio..FY0.');
data.addColumn('number','Current.Ratio..FY0.');
data.addColumn('number','Total.Assets..Reported..FY0..USD.');
data.addColumn('number','Dividend.yield');
data.addColumn('number','Revenue..FY0..USD.');
data.addColumn('number','Net.Income.After.Taxes..FY0..USD.');
data.addColumn('number','Capital.Expenditures..FY0..USD.');
data.addColumn('number','Retained.Earnings..TTM..FI0..USD.');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID2704c4757d2() {
var data = gvisDataTableID2704c4757d2();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1920;
options["height"] =    400;
options["frozenColumns"] =      1;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID2704c4757d2')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID2704c4757d2);
})();
function displayChartTableID2704c4757d2() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID2704c4757d2"></script>
 
<!-- divChart -->
  
<div id="TableID2704c4757d2" 
  style="width: 1920; height: 400;">
</div>
</div>
</div>
<br> <br>

Our Approach
---------------------------------------------------

#### Factor Analysis in 6 steps

1. Confirm the data in metric 

2. Decide whether to scale or standardize the data

3. Check the correlation matrix to see if Factor Analysis makes sense

4. Develop a scree plot and decide on the number of factors to be derived

5. Interpret the factors (consider factor rotations - technical but useful)

6. Save factor scores for subsequent analyses

Let's follow these steps.


The data we use here have the following descriptive statistics: 

<div class="row">
<div class="col-md-40">
<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID27044438b89a () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Company Market Cap  USD ",
0,
2067669.17,
6726472.43,
68577469.33,
24659227.59,
7358534619,
411725511.6 
],
[
 "Historic P E  FY0 ",
0,
0,
6.45,
24.04,
11.31,
3360.49,
155.18 
],
[
 "Total Debt to Total Equity  Percent  FY0 ",
0,
0,
0.13,
1.48,
0.8,
525.42,
18.2 
],
[
 "Enterprise Value To EBITDA  Daily Time Series Ratio ",
-214,
0,
4.36,
37.3,
8.39,
26770.95,
852.05 
],
[
 "Enterprise Value To Sales  Daily Time Series Ratio ",
-45.92,
0,
0.44,
1.44,
1.16,
133.32,
6.45 
],
[
 "P E  Daily Time Series Ratio ",
0,
0,
6.35,
16.87,
11.54,
2081.77,
94.38 
],
[
 "Total Debt To Enterprise Value  Daily Time Series Ratio ",
0,
0,
0.19,
0.32,
0.57,
6.16,
0.4 
],
[
 "Enterprise Value  Daily Time Series   USD ",
-36870373.69,
856323.12,
7436027.62,
76173044.19,
33952205.48,
6983632759,
416233961.8 
],
[
 "Price To Book Value Per Share  Daily Time Series Ratio ",
-16.36,
0.29,
0.71,
1.93,
1.25,
980.38,
31.14 
],
[
 "Quick Ratio  FY0 ",
0,
0,
0.71,
1.85,
1.44,
145.1,
7.7 
],
[
 "Current Ratio  FY0 ",
0,
0,
1.16,
2.28,
2.05,
145.1,
7.75 
],
[
 "Total Assets  Reported  FY0  USD ",
0,
3524663.5,
15219325.66,
223939799.5,
50168690.33,
37841176560,
2020011119 
],
[
 "Dividend yield",
0,
0,
0.02,
0.05,
0.07,
4.44,
0.21 
],
[
 "Revenue  FY0  USD ",
-257861.01,
1594496.41,
9981253.59,
48014704.38,
34296961.98,
2860329361,
164293729.7 
],
[
 "Net Income After Taxes  FY0  USD ",
-45360674.08,
0,
291893.08,
4629789.85,
2036698.94,
392888163.6,
25375183.36 
],
[
 "Capital Expenditures  FY0  USD ",
-645677007.1,
-1285301.45,
-163081.2,
-4558697.38,
0,
148622.62,
28078310.42 
],
[
 "Retained Earnings  TTM  FI0  USD ",
-27862390.34,
0,
126004.13,
3233360.07,
1445529.68,
232317103.8,
16326777.21 
] 
];
data.addColumn('string','Variables');
data.addColumn('number','min');
data.addColumn('number','X25.percent');
data.addColumn('number','median');
data.addColumn('number','mean');
data.addColumn('number','X75.percent');
data.addColumn('number','max');
data.addColumn('number','std');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID27044438b89a() {
var data = gvisDataTableID27044438b89a();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1920;
options["height"] =    400;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID27044438b89a')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID27044438b89a);
})();
function displayChartTableID27044438b89a() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID27044438b89a"></script>
 
<!-- divChart -->
  
<div id="TableID27044438b89a" 
  style="width: 1920; height: 400;">
</div>
</div>
</div>

#### Step 2: Decide whether to scale or standardize the data

We scaled the data because of the different magnitude of the numbers in the data under consideration.


```r
ProjectDatafactor_scaled=apply(ProjectDataFactor,2, function(r) {if (sd(r)!=0||is.na(r)==FALSE) res=(r-mean(r))/sd(r) else res=0*r; res})
```

Below is the summary statistics of the scaled dataset:

<br>


<div class="row">
<div class="col-md-40">
<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID270459be6235 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Company Market Cap  USD ",
-0.17,
-0.16,
-0.15,
0,
-0.11,
17.71,
1 
],
[
 "Historic P E  FY0 ",
-0.15,
-0.15,
-0.11,
0,
-0.08,
21.5,
1 
],
[
 "Total Debt to Total Equity  Percent  FY0 ",
-0.08,
-0.08,
-0.07,
0,
-0.04,
28.79,
1 
],
[
 "Enterprise Value To EBITDA  Daily Time Series Ratio ",
-0.29,
-0.04,
-0.04,
0,
-0.03,
31.38,
1 
],
[
 "Enterprise Value To Sales  Daily Time Series Ratio ",
-7.34,
-0.22,
-0.15,
0,
-0.04,
20.45,
1 
],
[
 "P E  Daily Time Series Ratio ",
-0.18,
-0.18,
-0.11,
0,
-0.06,
21.88,
1 
],
[
 "Total Debt To Enterprise Value  Daily Time Series Ratio ",
-0.81,
-0.81,
-0.34,
0,
0.61,
14.57,
1 
],
[
 "Enterprise Value  Daily Time Series   USD ",
-0.27,
-0.18,
-0.17,
0,
-0.1,
16.6,
1 
],
[
 "Price To Book Value Per Share  Daily Time Series Ratio ",
-0.59,
-0.05,
-0.04,
0,
-0.02,
31.42,
1 
],
[
 "Quick Ratio  FY0 ",
-0.24,
-0.24,
-0.15,
0,
-0.05,
18.6,
1 
],
[
 "Current Ratio  FY0 ",
-0.29,
-0.29,
-0.14,
0,
-0.03,
18.42,
1 
],
[
 "Total Assets  Reported  FY0  USD ",
-0.11,
-0.11,
-0.1,
0,
-0.09,
18.62,
1 
],
[
 "Dividend yield",
-0.25,
-0.25,
-0.16,
0,
0.09,
21.23,
1 
],
[
 "Revenue  FY0  USD ",
-0.29,
-0.28,
-0.23,
0,
-0.08,
17.12,
1 
],
[
 "Net Income After Taxes  FY0  USD ",
-1.97,
-0.18,
-0.17,
0,
-0.1,
15.3,
1 
],
[
 "Capital Expenditures  FY0  USD ",
-22.83,
0.12,
0.16,
0,
0.16,
0.17,
1 
],
[
 "Retained Earnings  TTM  FI0  USD ",
-1.9,
-0.2,
-0.19,
0,
-0.11,
14.03,
1 
] 
];
data.addColumn('string','Variables');
data.addColumn('number','min');
data.addColumn('number','X25.percent');
data.addColumn('number','median');
data.addColumn('number','mean');
data.addColumn('number','X75.percent');
data.addColumn('number','max');
data.addColumn('number','std');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID270459be6235() {
var data = gvisDataTableID270459be6235();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1920;
options["height"] =    400;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID270459be6235')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID270459be6235);
})();
function displayChartTableID270459be6235() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID270459be6235"></script>
 
<!-- divChart -->
  
<div id="TableID270459be6235" 
  style="width: 1920; height: 400;">
</div>
</div>
</div>

<br>
As expected all variables have mean 0 and standard deviation 1. 



#### Step 3:  Check correlation matrix to see if Factor Analysis makes sense

This is the correlation matrix of the 17 original variable we use for factor analysis. Some of the variables have strong correlations. The most obvious ones are between size meters such as revenue and value metrics such as market capitalization. Some interesting observations can be made from correlations alone. For instance dividend yield does not significantly affect valuation or depend on size. P/E does not depend on size. 

<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID2704129675cb () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 1,
0,
-0.01,
0,
0.04,
0.01,
-0.06,
0.96,
0,
0.01,
0.01,
0.58,
-0.02,
0.63,
0.85,
-0.53,
0.82 
],
[
 0,
1,
-0.01,
0.01,
0.03,
0.21,
0.01,
0,
0,
0.03,
0.02,
0,
-0.03,
-0.01,
-0.01,
0,
-0.01 
],
[
 -0.01,
-0.01,
1,
0,
0.01,
-0.01,
0.1,
-0.01,
0.02,
-0.01,
-0.02,
-0.01,
-0.01,
0,
-0.01,
0,
-0.01 
],
[
 0,
0.01,
0,
1,
0.11,
0.07,
-0.02,
0,
0,
0.06,
0.06,
0,
-0.01,
-0.01,
-0.01,
0,
-0.01 
],
[
 0.04,
0.03,
0.01,
0.11,
1,
0.01,
0.06,
0.05,
0,
0,
0.01,
0,
-0.03,
-0.01,
0.01,
-0.03,
0.01 
],
[
 0.01,
0.21,
-0.01,
0.07,
0.01,
1,
0.01,
0.02,
0,
0,
0,
0.01,
-0.03,
0.01,
0,
-0.02,
-0.01 
],
[
 -0.06,
0.01,
0.1,
-0.02,
0.06,
0.01,
1,
-0.02,
0.05,
-0.09,
-0.09,
-0.05,
0.02,
0.06,
-0.07,
-0.03,
-0.06 
],
[
 0.96,
0,
-0.01,
0,
0.05,
0.02,
-0.02,
1,
0.01,
0,
0,
0.47,
-0.02,
0.69,
0.77,
-0.68,
0.74 
],
[
 0,
0,
0.02,
0,
0,
0,
0.05,
0.01,
1,
0,
0,
0,
0,
0.01,
0.01,
0,
0.01 
],
[
 0.01,
0.03,
-0.01,
0.06,
0,
0,
-0.09,
0,
0,
1,
1,
-0.02,
-0.02,
-0.02,
-0.01,
0.01,
-0.02 
],
[
 0.01,
0.02,
-0.02,
0.06,
0.01,
0,
-0.09,
0,
0,
1,
1,
-0.02,
-0.02,
-0.02,
-0.01,
0.01,
-0.02 
],
[
 0.58,
0,
-0.01,
0,
0,
0.01,
-0.05,
0.47,
0,
-0.02,
-0.02,
1,
-0.02,
0.08,
0.62,
-0.24,
0.78 
],
[
 -0.02,
-0.03,
-0.01,
-0.01,
-0.03,
-0.03,
0.02,
-0.02,
0,
-0.02,
-0.02,
-0.02,
1,
-0.01,
-0.01,
0.02,
-0.02 
],
[
 0.63,
-0.01,
0,
-0.01,
-0.01,
0.01,
0.06,
0.69,
0.01,
-0.02,
-0.02,
0.08,
-0.01,
1,
0.64,
-0.57,
0.51 
],
[
 0.85,
-0.01,
-0.01,
-0.01,
0.01,
0,
-0.07,
0.77,
0.01,
-0.01,
-0.01,
0.62,
-0.01,
0.64,
1,
-0.41,
0.88 
],
[
 -0.53,
0,
0,
0,
-0.03,
-0.02,
-0.03,
-0.68,
0,
0.01,
0.01,
-0.24,
0.02,
-0.57,
-0.41,
1,
-0.41 
],
[
 0.82,
-0.01,
-0.01,
-0.01,
0.01,
-0.01,
-0.06,
0.74,
0.01,
-0.02,
-0.02,
0.78,
-0.02,
0.51,
0.88,
-0.41,
1 
] 
];
data.addColumn('number','Company.Market.Cap..USD.');
data.addColumn('number','Historic.P.E..FY0.');
data.addColumn('number','Total.Debt.to.Total.Equity..Percent..FY0.');
data.addColumn('number','Enterprise.Value.To.EBITDA..Daily.Time.Series.Ratio.');
data.addColumn('number','Enterprise.Value.To.Sales..Daily.Time.Series.Ratio.');
data.addColumn('number','P.E..Daily.Time.Series.Ratio.');
data.addColumn('number','Total.Debt.To.Enterprise.Value..Daily.Time.Series.Ratio.');
data.addColumn('number','Enterprise.Value..Daily.Time.Series...USD.');
data.addColumn('number','Price.To.Book.Value.Per.Share..Daily.Time.Series.Ratio.');
data.addColumn('number','Quick.Ratio..FY0.');
data.addColumn('number','Current.Ratio..FY0.');
data.addColumn('number','Total.Assets..Reported..FY0..USD.');
data.addColumn('number','Dividend.yield');
data.addColumn('number','Revenue..FY0..USD.');
data.addColumn('number','Net.Income.After.Taxes..FY0..USD.');
data.addColumn('number','Capital.Expenditures..FY0..USD.');
data.addColumn('number','Retained.Earnings..TTM..FI0..USD.');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID2704129675cb() {
var data = gvisDataTableID2704129675cb();
var options = {};
options["allowHtml"] = true;
options["width"] =   1920;
options["height"] =    400;
options["allowHTML"] = true;

    var chart = new google.visualization.Table(
    document.getElementById('TableID2704129675cb')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID2704129675cb);
})();
function displayChartTableID2704129675cb() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID2704129675cb"></script>
 
<!-- divChart -->
  
<div id="TableID2704129675cb" 
  style="width: 1920; height: 400;">
</div>


#### Step 4. Develop a scree plot and decide on the number of factors to be derived

Based on the cumulative explained variance we use six components that explain 67% of the total variance.

<br>

<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID27044078ccf0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Component No:1",
4.785247641,
28.14851553,
28.14851553 
],
[
 "Component No:2",
2.025465294,
11.91450173,
40.06301727 
],
[
 "Component No:3",
1.261235076,
7.419029856,
47.48204712 
],
[
 "Component No:4",
1.216184347,
7.154025572,
54.63607269 
],
[
 "Component No:5",
1.091912549,
6.423014997,
61.05908769 
],
[
 "Component No:6",
1.059107436,
6.230043743,
67.28913143 
],
[
 "Component No:7",
0.996303332,
5.860607835,
73.14973927 
],
[
 "Component No:8",
0.9818763148,
5.775743028,
78.9254823 
],
[
 "Component No:9",
0.9174703742,
5.396884554,
84.32236685 
],
[
 "Component No:10",
0.8379317778,
4.929010458,
89.25137731 
],
[
 "Component No:11",
0.7736384203,
4.550814237,
93.80219155 
],
[
 "Component No:12",
0.5560328789,
3.270781641,
97.07297319 
],
[
 "Component No:13",
0.282367605,
1.660985911,
98.7339591 
],
[
 "Component No:14",
0.1156329954,
0.6801940907,
99.41415319 
],
[
 "Component No:15",
0.08375688055,
0.4926875327,
99.90684072 
],
[
 "Component No:16",
0.01169527521,
0.06879573654,
99.97563646 
],
[
 "Component No:17",
0.004141802172,
0.02436354219,
100 
] 
];
data.addColumn('string','Components');
data.addColumn('number','Eigenvalue');
data.addColumn('number','Percentage_of_explained_variance');
data.addColumn('number','Cumulative_percentage_of_explained_variance');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID27044078ccf0() {
var data = gvisDataTableID27044078ccf0();
var options = {};
options["allowHtml"] = true;
options["width"] =   1200;
options["height"] =    400;
options["allowHTML"] = true;
options["page"] = "disable";

  var dataFormat1 = new google.visualization.NumberFormat({pattern:"#.##"});
  dataFormat1.format(data, 1);
  var dataFormat2 = new google.visualization.NumberFormat({pattern:"#.##"});
  dataFormat2.format(data, 2);
  var dataFormat3 = new google.visualization.NumberFormat({pattern:"#.##"});
  dataFormat3.format(data, 3);

    var chart = new google.visualization.Table(
    document.getElementById('TableID27044078ccf0')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID27044078ccf0);
})();
function displayChartTableID27044078ccf0() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID27044078ccf0"></script>
 
<!-- divChart -->
  
<div id="TableID27044078ccf0" 
  style="width: 1200; height: 400;">
</div>
<br> <br>


<!-- LineChart generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataLineChartID270469424f34 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "1",
4.785247641,
1 
],
[
 "2",
2.025465294,
1 
],
[
 "3",
1.261235076,
1 
],
[
 "4",
1.216184347,
1 
],
[
 "5",
1.091912549,
1 
],
[
 "6",
1.059107436,
1 
],
[
 "7",
0.996303332,
1 
],
[
 "8",
0.9818763148,
1 
],
[
 "9",
0.9174703742,
1 
],
[
 "10",
0.8379317778,
1 
],
[
 "11",
0.7736384203,
1 
],
[
 "12",
0.5560328789,
1 
],
[
 "13",
0.282367605,
1 
],
[
 "14",
0.1156329954,
1 
],
[
 "15",
0.08375688055,
1 
],
[
 "16",
0.01169527521,
1 
],
[
 "17",
0.004141802172,
1 
] 
];
data.addColumn('string','components');
data.addColumn('number','eigenvalues');
data.addColumn('number','abline');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartLineChartID270469424f34() {
var data = gvisDataLineChartID270469424f34();
var options = {};
options["allowHtml"] = true;
options["title"] = "Scree plot";
options["legend"] = "right";
options["width"] =    900;
options["height"] =    600;
options["hAxis"] = {title:'Number of Components', titleTextStyle:{color:'black'}};
options["vAxes"] = [{title:'Eigenvalues'}];
options["series"] = [{color:'green',pointSize:3, targetAxisIndex: 0}];

    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID270469424f34')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartLineChartID270469424f34);
})();
function displayChartLineChartID270469424f34() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID270469424f34"></script>
 
<!-- divChart -->
  
<div id="LineChartID270469424f34" 
  style="width: 900; height: 600;">
</div>




#### 5. Interpret the factors 

For our data, the selected factors look as follows after the rotation: 

<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:55 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID27043420d96c () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Revenue  FY0  USD ",
0.89,
0.1,
-0.01,
-0.02,
-0.05,
0.01 
],
[
 "Enterprise Value  Daily Time Series   USD ",
0.8,
0.51,
0.01,
0.01,
0.03,
-0.01 
],
[
 "Company Market Cap  USD ",
0.68,
0.66,
0.02,
0.01,
0.02,
-0.03 
],
[
 "Net Income After Taxes  FY0  USD ",
0.56,
0.73,
0,
-0.01,
0,
-0.02 
],
[
 "Retained Earnings  TTM  FI0  USD ",
0.45,
0.85,
-0.02,
-0.01,
0,
-0.01 
],
[
 "Total Debt To Enterprise Value  Daily Time Series Ratio ",
0.17,
-0.23,
-0.13,
0.04,
0.09,
0.62 
],
[
 "Enterprise Value To Sales  Daily Time Series Ratio ",
0.05,
-0.02,
-0.03,
-0.02,
0.76,
0.08 
],
[
 "Dividend yield",
0.04,
-0.08,
-0.03,
-0.15,
-0.16,
-0.05 
],
[
 "P E  Daily Time Series Ratio ",
0.03,
-0.02,
-0.02,
0.77,
0.06,
-0.03 
],
[
 "Total Assets  Reported  FY0  USD ",
0.03,
0.92,
-0.03,
0.03,
0.03,
0.03 
],
[
 "Historic P E  FY0 ",
0,
-0.01,
0.02,
0.77,
-0.03,
0.01 
],
[
 "Quick Ratio  FY0 ",
0,
-0.01,
1,
0.01,
0.03,
-0.01 
],
[
 "Current Ratio  FY0 ",
0,
-0.01,
1,
0.01,
0.03,
-0.01 
],
[
 "Enterprise Value To EBITDA  Daily Time Series Ratio ",
-0.01,
-0.01,
0.06,
0.05,
0.71,
-0.12 
],
[
 "Price To Book Value Per Share  Daily Time Series Ratio ",
-0.04,
0.06,
0.04,
0,
-0.05,
0.46 
],
[
 "Total Debt to Total Equity  Percent  FY0 ",
-0.06,
0.06,
0.02,
-0.02,
0.01,
0.71 
],
[
 "Capital Expenditures  FY0  USD ",
-0.8,
-0.09,
0.01,
-0.01,
-0.01,
0 
] 
];
data.addColumn('string','Variables');
data.addColumn('number','Component 1');
data.addColumn('number','Component 2');
data.addColumn('number','Component 3');
data.addColumn('number','Component 4');
data.addColumn('number','Component 5');
data.addColumn('number','Component 6');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID27043420d96c() {
var data = gvisDataTableID27043420d96c();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1220;
options["height"] =    400;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID27043420d96c')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID27043420d96c);
})();
function displayChartTableID27043420d96c() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID27043420d96c"></script>
 
<!-- divChart -->
  
<div id="TableID27043420d96c" 
  style="width: 1220; height: 400;">
</div>
<br> <br>

Component 1 mainly consists of size metrics from recent performance and value metrics. Component 2 has some more longer time size metrics. It Component 3 consists of two debt capacity metrics. Component 4 combines historical and current p/e ratios. Component 5 has two variables that measure the valuation in relation to performance. Component 6 groups two metrics of debt to assets.

Components 1 and 2 have somewhat similar loadings because all the variables correlate strongly with each other. It might not make sense to use both of them.

<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:56 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID2704b5280c6 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Revenue  FY0  USD ",
0.89,
null,
null,
null,
null,
null 
],
[
 "Enterprise Value  Daily Time Series   USD ",
0.8,
0.51,
null,
null,
null,
null 
],
[
 "Company Market Cap  USD ",
0.68,
0.66,
null,
null,
null,
null 
],
[
 "Net Income After Taxes  FY0  USD ",
0.56,
0.73,
null,
null,
null,
null 
],
[
 "Retained Earnings  TTM  FI0  USD ",
null,
0.85,
null,
null,
null,
null 
],
[
 "Total Debt To Enterprise Value  Daily Time Series Ratio ",
null,
null,
null,
null,
null,
0.62 
],
[
 "Enterprise Value To Sales  Daily Time Series Ratio ",
null,
null,
null,
null,
0.76,
null 
],
[
 "Dividend yield",
null,
null,
null,
null,
null,
null 
],
[
 "P E  Daily Time Series Ratio ",
null,
null,
null,
0.77,
null,
null 
],
[
 "Total Assets  Reported  FY0  USD ",
null,
0.92,
null,
null,
null,
null 
],
[
 "Historic P E  FY0 ",
null,
null,
null,
0.77,
null,
null 
],
[
 "Quick Ratio  FY0 ",
null,
null,
1,
null,
null,
null 
],
[
 "Current Ratio  FY0 ",
null,
null,
1,
null,
null,
null 
],
[
 "Enterprise Value To EBITDA  Daily Time Series Ratio ",
null,
null,
null,
null,
0.71,
null 
],
[
 "Price To Book Value Per Share  Daily Time Series Ratio ",
null,
null,
null,
null,
null,
null 
],
[
 "Total Debt to Total Equity  Percent  FY0 ",
null,
null,
null,
null,
null,
0.71 
],
[
 "Capital Expenditures  FY0  USD ",
-0.8,
null,
null,
null,
null,
null 
] 
];
data.addColumn('string','Variables');
data.addColumn('number','Component 1');
data.addColumn('number','Component 2');
data.addColumn('number','Component 3');
data.addColumn('number','Component 4');
data.addColumn('number','Component 5');
data.addColumn('number','Component 6');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID2704b5280c6() {
var data = gvisDataTableID2704b5280c6();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1220;
options["height"] =    400;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID2704b5280c6')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID2704b5280c6);
})();
function displayChartTableID2704b5280c6() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID2704b5280c6"></script>
 
<!-- divChart -->
  
<div id="TableID2704b5280c6" 
  style="width: 1220; height: 400;">
</div>
<br> <br>


#### Step 6. Save factor scores for subsequent analyses

For our data, using the rotated factors we selected, we can create a new dataset where our observations are as follows (for the first 50 companies):

<div class="row">
<div class="col-md-40">

<!-- Table generated in R 3.3.0 by googleVis 0.5.10 package -->
<!-- Wed Jun 15 21:58:56 2016 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID270460d959a4 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "1",
0.08,
0.21,
-0.11,
-0.16,
0.39,
0.11 
],
[
 "2",
-0.31,
0.02,
-0.22,
-0.18,
-0.18,
-0.18 
],
[
 "3",
1.12,
-0.6,
-0.2,
0.12,
-0.15,
0.43 
],
[
 "4",
-0.16,
-0.14,
-0.16,
-0.13,
-0.14,
0.13 
],
[
 "5",
-0.05,
-0.26,
-0.2,
-0.09,
0.02,
0.65 
],
[
 "6",
0.08,
-0.25,
-0.19,
-0.15,
-0.05,
0.45 
],
[
 "7",
-0.32,
0.04,
0.15,
-0.14,
-0.05,
-0.48 
],
[
 "8",
-0.27,
-0.02,
0.1,
-0.09,
0.03,
-0.33 
],
[
 "9",
-0.29,
0,
0.09,
-0.12,
-0.1,
-0.31 
],
[
 "10",
-0.21,
-0.07,
-0.25,
-0.23,
-0.21,
-0.23 
],
[
 "11",
-0.25,
0.04,
0,
-0.15,
-0.19,
-0.49 
],
[
 "12",
-0.26,
0,
-0.22,
-0.22,
-0.23,
-0.52 
],
[
 "13",
0,
-0.29,
-0.09,
-0.19,
-0.12,
0.5 
],
[
 "14",
-0.08,
-0.22,
-0.17,
0.36,
-0.1,
0.43 
],
[
 "15",
0.19,
-0.17,
-0.21,
-0.17,
0.04,
0.59 
],
[
 "16",
0,
0.69,
-0.18,
-0.18,
0.2,
0.3 
],
[
 "17",
0.03,
-0.33,
-0.33,
-0.12,
-0.02,
0.8 
],
[
 "18",
-0.28,
-0.01,
-0.11,
-0.21,
-0.24,
-0.42 
],
[
 "19",
-0.35,
0.05,
-0.22,
-0.19,
-0.18,
-0.52 
],
[
 "20",
-0.19,
0,
0.19,
-0.11,
-0.21,
-0.48 
],
[
 "21",
-0.04,
-0.27,
-0.43,
1.6,
1.61,
0.37 
],
[
 "22",
0.27,
-0.4,
-0.25,
0.1,
0,
0.8 
],
[
 "23",
-0.14,
-0.3,
0,
-0.22,
0.69,
0.2 
],
[
 "24",
-0.31,
0.02,
-0.11,
-0.2,
-0.32,
-0.53 
],
[
 "25",
-0.37,
0.09,
-0.22,
-0.18,
-0.18,
-0.51 
],
[
 "26",
-0.27,
0.02,
-0.22,
-0.22,
-0.23,
-0.49 
],
[
 "27",
-0.13,
-0.09,
0.13,
-0.02,
-0.05,
-0.02 
],
[
 "28",
-0.31,
0.01,
0.27,
-0.24,
-0.27,
-0.5 
],
[
 "29",
0.07,
-0.41,
-0.35,
-0.1,
0.02,
1.08 
],
[
 "30",
-0.29,
0,
-0.09,
-0.05,
-0.19,
-0.41 
],
[
 "31",
-0.05,
-0.27,
-0.15,
0.05,
0.05,
0.7 
],
[
 "32",
-0.31,
0.03,
-0.05,
0.42,
-0.03,
-0.47 
],
[
 "33",
-0.25,
-0.01,
-0.2,
0.24,
2.16,
-0.3 
],
[
 "34",
0.03,
-0.31,
-0.17,
-0.08,
-0.05,
0.61 
],
[
 "35",
0.47,
-0.89,
-0.26,
-2.03,
-2.25,
-1.23 
],
[
 "36",
-0.24,
0.04,
-0.16,
-0.13,
0.14,
-0.34 
],
[
 "37",
-0.28,
0.06,
1.08,
-0.19,
0.01,
-0.38 
],
[
 "38",
-0.09,
-0.22,
-0.3,
-0.22,
-0.17,
0.27 
],
[
 "39",
-0.23,
0.01,
-0.16,
-0.14,
-0.12,
-0.15 
],
[
 "40",
-0.15,
-0.14,
-0.18,
0.22,
-0.09,
0.08 
],
[
 "41",
0.1,
-0.15,
-0.14,
-0.16,
-0.14,
0.01 
],
[
 "42",
0.12,
-0.33,
-0.22,
-0.16,
0,
0.37 
],
[
 "43",
-0.04,
-0.3,
-0.29,
-0.86,
-0.94,
-0.78 
],
[
 "44",
-0.27,
0,
-0.22,
-0.22,
-0.22,
-0.49 
],
[
 "45",
-0.04,
-0.1,
-0.16,
-0.09,
0.09,
0.02 
],
[
 "46",
-0.33,
0.03,
-0.23,
-0.24,
-0.24,
-0.54 
],
[
 "47",
-0.07,
-0.22,
-0.15,
-0.15,
-0.09,
0.35 
],
[
 "48",
0.12,
-0.31,
-0.2,
-0.19,
-0.11,
0.55 
],
[
 "49",
0.14,
-0.44,
-0.35,
-0.15,
-0.05,
0.97 
],
[
 "50",
-0.24,
0.19,
0.09,
-0.15,
-0.04,
-0.45 
] 
];
data.addColumn('string','Observation');
data.addColumn('number','Derived Variable (Factor) 1');
data.addColumn('number','Derived Variable (Factor) 2');
data.addColumn('number','Derived Variable (Factor) 3');
data.addColumn('number','Derived Variable (Factor) 4');
data.addColumn('number','Derived Variable (Factor) 5');
data.addColumn('number','Derived Variable (Factor) 6');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID270460d959a4() {
var data = gvisDataTableID270460d959a4();
var options = {};
options["allowHtml"] = true;
options["showRowNumber"] = true;
options["width"] =   1220;
options["height"] =    400;
options["frozenColumns"] =      1;
options["allowHTML"] = true;
options["page"] = "disable";

    var chart = new google.visualization.Table(
    document.getElementById('TableID270460d959a4')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID270460d959a4);
})();
function displayChartTableID270460d959a4() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID270460d959a4"></script>
 
<!-- divChart -->
  
<div id="TableID270460d959a4" 
  style="width: 1220; height: 400;">
</div>
</div>
</div>
<br> <br>

Further Ideas
---------------------------------------------------------------

This framework can be extended to work as a tool for screening companies. It would make sense to add a lot more variables. Then components can be compared with other markets to test hypothesis along the lines “does debt capacity matter more or less for valuation in these markets?” The framework can also be extended for back testing investment strategies. 
