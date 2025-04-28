# comp9313---assignment-2-spark-solved
**TO GET THIS SOLUTION VISIT:** [COMP9313 – Assignment #2 (Spark) Solved](https://www.ankitcodinghub.com/product/comp9313-assignment-2-spark-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;44208&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP9313 -  Assignment #2 (Spark) Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<span style="font-size: 2.61792em; letter-spacing: -1px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Problem Statement</span>

&nbsp;

Given a log file that records HTTP requests (GET and POST) sent to a set of servers, you are asked to compute descriptive statistics on the amount of data (payload) communicated through such requests. These statistics need to be computed for each base URL (e.g., “http://subdom0001. example.com”)&nbsp; in the log and the results must be reported in bytes.&nbsp; More specifically, you need to compute the following statistics per each sub-domain):

&nbsp;

<strong><em>Minimum payload: </em></strong>The smallest payload communicated for each base URL.

&nbsp;

<strong><em>Maximum payload:</em></strong> The largest payload communicated for each base URL.

&nbsp;

<strong><em>Mean payload:</em></strong> Mean of payloads for each base URL. For computing the mean, consider the following formula (population mean):

&nbsp;

&nbsp;

&nbsp;

where N is the size of the population being explored.

<strong><em>&nbsp;</em></strong>

<strong><em>&nbsp;</em></strong>

<strong><em>Variance of payload:</em></strong> The variance of payloads for each base URL. For computing the variance, consider the following formula (population variance):

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

where N is the population size and 𝜇 is the population mean.

&nbsp;

Notice that the statistics above need to be computed for each base URL in the log.

&nbsp;

You are asked to develop a Spark solution to this problem (using Scala). Your solution must be runnable using the <em>spark-shell</em> interpreter. Your solution must rely on <strong>RDDs</strong> to solve this problem (the use Spark DataFrames and DataSets are <strong><em>not allowed</em></strong> for this assignment).

&nbsp;

<h1>2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Input</h1>
<strong>&nbsp;</strong>

The log file in input is a CSV file that contains one line HTTP per request. The file consists of three columns: Base URL of the HTTP request, endpoint, HTTP method, and size of payload. An excerpt of the log is shown below:

&nbsp;

&nbsp;

http://subdom0001.example.com,/endpoint0001,POST,3B http://subdom0002.example.com,/endpoint0002,GET,431MB http://subdom0003.example.com,/endpoint0003,POST,231KB http://subdom0002.example.com,/endpoint0002,GET,29MB http://subdom0001.example.com,/endpoint0001,POST,238B http://subdom0002.example.com,/endpoint0001,GET,32MB http://subdom0003.example.com,/endpoint0003,GET,21KB Notice that the payload is given in different units of digital information (e.g. MB and KB). The log file for this assignment will contain the following units only: B (for bytes), KB (for kilobytes) and MB (for megabytes).

&nbsp;

Assume that the log file is stored in a local filesystem (we will not use HDFS or similar for this assignment). We provide a sample log file in the link below:

<a href="https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28426">https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28426</a>

<strong>&nbsp;</strong>

&nbsp;

<h1>3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Output</h1>
&nbsp;

The output consists in a CSV file that contains the list of base URLs along with the descriptive statistics (for each base URL)&nbsp; as presented in Section 1. We show a sample output below:

&nbsp;

&nbsp;

http://subdom0001.example.com,3B,238B,120B,13806B

http://subdom0002.example.com,30408704B,451936256B,171966464B,39193191483703296B http://subdom0003.example.com,21504B,236544B,129024B,11560550400B

&nbsp;

&nbsp;

The columns in the output above are as follows: Base URL, minimum payload, maximum payload, mean payload, variance of payload. You do not need to provide a <em>header</em> for your CSV file.

&nbsp;

Notice that the statistics must be expressed in bytes (B), as shown in the example above. Note also that you may get float / double numbers when computing means and variance. In such cases, <em>truncate</em> the numbers to keep just the whole number part. For example:

&nbsp;

<ul>
<li>32 -&gt; 120938</li>
<li>89 -&gt; 9983</li>
</ul>
&nbsp;

We provide a sample output in the URL below:

<a href="https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28428">https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28428</a>

&nbsp;

&nbsp;

<strong>&nbsp; </strong>

&nbsp;

&nbsp;

<h1>4 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Input file and output file specification</h1>
&nbsp;

You will need to specify (in your Scala program) the path of your input file and output directory (where the results file will be stored) using two Scala values (<em>val</em>) with the following names:

&nbsp;

val inputFilePath = “FULL_PATH_OF_YOUR_INPUT_FILE”

&nbsp;

val outputDirPath = “FULL_PATH_OF_YOUR_OUTPUT_DIRECTORY”

&nbsp;

Use this value names (inputFilePath and outputDirPath) whenever you need to read/write the input/output.

&nbsp;

During assessment, we will change these values to the path of the input file and output directory used for assessing your work.

&nbsp;

Please, locate the declaration of these values at the very beginning of your program. You can use the code template provided in the link below to write your solution:

&nbsp;

<a href="https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28425"><strong>&nbsp;</strong></a><a href="https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28425">https://webcms3.cse.unsw.edu.au/COMP9313/19T2/resources/28425</a>

&nbsp;

<h1>5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Running your Program</h1>
&nbsp;

We will run your program using spark-shell. More specifically, we will use the following command to load and run your Scala program:

&nbsp;

<strong>scala&gt;</strong> :load assignment2.scala

&nbsp;

&nbsp;

&nbsp;

<strong>&nbsp;</strong>

<h1>6 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assignment Submission</h1>
<strong>&nbsp;</strong>

<strong><em>Deadline:</em></strong> 21 July 2019 20:59:59

&nbsp;

Log in to any CSE server (e.g. williams or wagner) and use the <em>give command</em> below to submit your solution:

&nbsp;

$ give cs9313 assignment2 z9999999.zip

&nbsp;

where you must replace z9999999 above with your own zID. The zip file above must contain the following:

<ul>
<li>The file assignment2.scala containing your solution (Scala program)</li>
<li>A PDF document, named assignment2_solution.pdf (maximum 1 page, 10 points font-size Arial), that explains your solution (use of figures is highly encouraged to explain your solution).</li>
</ul>
&nbsp;

You can also submit your solution using WebCMS, or Give:

&nbsp;

<a href="https://cgi.cse.unsw.edu.au/~give/Student/give.php">https://cgi.cse.unsw.edu.au/~give/Student/give.php</a>

&nbsp;

If you submit your assignment more than once, the last submission will replace the previous one. The late submission penalty (below) will be applied based on the timestamp of your last submission. To prove successful submission, please take a screenshot and keep it for your own record. If you face any problem while submitting your code, please e-mail the Course Admin (Maisie Badami, m.badami@student.unsw.edu.au)

&nbsp;

<strong>7 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Late submission penalty </strong>

<strong>&nbsp;</strong>

10% reduction of your marks for the 1st day, 30% reduction/day for the following days.

<strong>&nbsp;</strong>

<h1>8 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assessment</h1>
&nbsp;

Your source code will be manually inspected and marked based on readability and ease of understanding. We will run your code to verify that it produces correct results. The code documentation (i.e. comments in your source code) and solution explanation (PDF document) are also important. Below, we provide an indicative assessment scheme (maximum mark: 25 points):

&nbsp;

<table width="350">
<tbody>
<tr>
<td width="225">Result correctness</td>
<td width="125">15 points</td>
</tr>
<tr>
<td width="225">Documentation (PDF document)</td>
<td width="125">5 points</td>
</tr>
<tr>
<td width="225">Code structure and source code documentation (comments)</td>
<td width="125">5 points</td>
</tr>
</tbody>
</table>
&nbsp;

&nbsp;
