<h2>Introduction</h2>

<p>It is now possible to collect a large amount of data about personal
movement using activity monitoring devices such as a
<a href="http://www.fitbit.com">Fitbit</a>, <a href="http://www.nike.com/us/en_us/c/nikeplus-fuelband">Nike
Fuelband</a>, or
<a href="https://jawbone.com/up">Jawbone Up</a>. These type of devices are part of
the “quantified self” movement – a group of enthusiasts who take
measurements about themselves regularly to improve their health, to
find patterns in their behavior, or because they are tech geeks. But
these data remain under-utilized both because the raw data are hard to
obtain and there is a lack of statistical methods and software for
processing and interpreting the data.</p>

<p>This assignment makes use of data from a personal activity monitoring
device. This device collects data at 5 minute intervals through out the
day. The data consists of two months of data from an anonymous
individual collected during the months of October and November, 2012
and include the number of steps taken in 5 minute intervals each day.</p>

<h2>Data</h2>

<p>The data for this assignment can be downloaded from the course web
site:</p>

<ul><li>Dataset: <a href="https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip">Activity monitoring data</a> [52K]</li>
</ul><p>The variables included in this dataset are:</p>

<ul><li><p><b>steps</b>: Number of steps taking in a 5-minute interval (missing
values are coded as <code>NA</code>)</p></li>
<li><p><b>date</b>: The date on which the measurement was taken in YYYY-MM-DD
format</p></li>
<li><p><b>interval</b>: Identifier for the 5-minute interval in which
measurement was taken</p></li>
</ul><p>The dataset is stored in a comma-separated-value (CSV) file and there
are a total of 17,568 observations in this
dataset.</p>

<h2>Assignment</h2>

<p>This assignment will be described in multiple parts. You will need to
write a report that answers the questions detailed below. Ultimately,
you will need to complete the entire assignment in a <b>single R
markdown</b> document that can be processed by <b>knitr</b> and be
transformed into an HTML file.</p>

<p>Throughout your report make sure you always include the code that you
used to generate the output you present. When writing code chunks in
the R markdown document, always use <code>echo = TRUE</code> so that someone else
will be able to read the code. <b>This assignment will be evaluated via
peer assessment so it is essential that your peer evaluators be able
to review the code for your analysis</b>.</p>

<p>For the plotting aspects of this assignment, feel free to use any
plotting system in R (i.e., base, lattice, ggplot2)</p>

<p>Fork/clone the <a href="http://github.com/rdpeng/RepData_PeerAssessment1">GitHub repository created for this
assignment</a>. You
will submit this assignment by pushing your completed files into your
forked repository on GitHub. The assignment submission will consist of
the URL to your GitHub repository and the SHA-1 commit ID for your
repository state.</p>

<p>NOTE: The GitHub repository also contains the dataset for the
assignment so you do not have to download the data separately.</p>

<h3>Loading and preprocessing the data</h3>

<p>Show any code that is needed to</p>

<ol><li><p>Load the data (i.e. <code>read.csv()</code>)</p></li>
<li><p>Process/transform the data (if necessary) into a format suitable for your analysis</p></li>
</ol><h3>What is mean total number of steps taken per day?</h3>

<p>For this part of the assignment, you can ignore the missing values in
the dataset.</p>

<ol><li><p>







</p><p>Calculate the total number of steps taken per day</p></li>
<li><p>







</p><p>If you do not understand the difference between a histogram and a barplot, research the difference between them. Make a histogram of the total number of steps taken each day</p></li><li><p><span>







</span></p><p><span>Calculate and report the mean and median of the total number of steps taken per day</span></p></li>
</ol><h3>What is the average daily activity pattern?</h3>

<ol><li><p>Make a time series plot (i.e. <code>type = "l"</code>) of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all days (y-axis)</p></li>
<li><p>Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?</p></li>
</ol><h3>Imputing missing values</h3>

<p>Note that there are a number of days/intervals where there are missing
values (coded as <code>NA</code>). The presence of missing days may introduce
bias into some calculations or summaries of the data.</p>

<ol><li><p>Calculate and report the total number of missing values in the dataset (i.e. the total number of rows with <code>NA</code>s)</p></li>
<li><p>Devise a strategy for filling in all of the missing values in the dataset. The strategy does not need to be sophisticated. For example, you could use the mean/median for that day, or the mean for that 5-minute interval, etc.</p></li>
<li><p>Create a new dataset that is equal to the original dataset but with the missing data filled in.</p></li>
<li><p>Make a histogram of the total number of steps taken each day and Calculate and report the <b>mean</b> and <b>median</b> total number of steps taken per day. Do these values differ from the estimates from the first part of the assignment? What is the impact of imputing missing data on the estimates of the total daily number of steps?</p></li>
</ol><h3>Are there differences in activity patterns between weekdays and weekends?</h3>

<p>For this part the <code>weekdays()</code> function may be of some help here. Use
the dataset with the filled-in missing values for this part.</p>

<ol><li><p>Create a new factor variable in the dataset with two levels – “weekday” and “weekend” indicating whether a given date is a weekday or weekend day.</p></li>
<li><p>Make a panel plot containing a time series plot (i.e. <code>type = "l"</code>) of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis). See the README file in the GitHub repository to see an example of what this plot should look like using simulated data.</p></li></ol><h2>Submitting the Assignment</h2>

<p>To submit the assignment:</p>

<ol><li><p>Commit the your completed <code>PA1_template.Rmd</code> file to the <code>master</code> branch of your git repository (you should already be on the <code>master</code> branch unless you created new ones)</p></li>
<li><p>







</p><p>Commit your PA1_template.md and PA1_template.html files produced by processing your R markdown file with knit2html() function in R (from the knitr package) by running the function from the console.</p></li>
<li><p>







</p><p>If your document has figures included (it should) then they should have been placed in the figure/ directory by default (unless you overrided the default). Add and commit the figure/ directory to yoru git repository so that the figures appear in the markdown file when it displays on github.</p></li>
<li><p>Push your <code>master</code> branch to GitHub.</p></li>
<li><p>Submit the URL to your GitHub repository for this assignment on the course web site.</p></li>
</ol><p>In addition to submitting the URL for your GitHub repository, you will
need to submit the 40 character SHA-1 hash (as string of numbers from
0-9 and letters from a-f) that identifies the repository commit that
contains the version of the files you want to submit. You can do this
in GitHub by doing the following</p>

<ol><li><p>Going to your GitHub repository web page for this assignment</p></li>
<li><p>Click on the “?? commits” link where ?? is the number of commits you have in the repository. For example, if you made a total of 10 commits to this repository, the link should say “10 commits”.</p></li>
<li><p>You will see a list of commits that you have made to this repository. The most recent commit is at the very top. If this represents the version of the files you want to submit, then just click the “copy to clipboard” button on the right hand side that should appear when you hover over the SHA-1 hash. Paste this SHA-1 hash into the course web site when you submit your assignment. If you don't want to use the most recent commit, then go down and find the commit you want and copy the SHA-1 hash.</p>
