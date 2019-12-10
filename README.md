# Live Project

<h2 style="color: blue;">Overview</h2>
<p>
The last two weeks of my time at the Tech Academy revolved around a live porject. Along with my peers we worked on fixing bugs, adding features, and updating the clients website. 
</p>

<p>We worked on a legacy code base which was begun by others before us. I worked on the front end (<b>HTML, CSS, JavaScript</b>) while others worked on the back end (<b>C# & Python</b>). Most of the CSS was done with vanilla CSS and <b>Bootstrap</b>. The software design pattern we used was MVC (<b>Model-Viewer-Controller</b>) which is what we will commonly see in the workplace. We used <b>Microsoft Azure DevOps</b> as our git repository and team workspace on the <b>Visual Studio</b> software. This taught me about the master branch vs other created branches, pulling, pushing, merging, and much more. We were able to assign ourselves 'stories' to complete for the project as is done in the software industry. We implemented the <b>SCRUM</b> method of sprints and daily stand-ups to keep everyone on the same page during the project. We were encouraged to treat this as a job and rely on one another through Slack or stand-ups if we needed help.
</p>

<p>
Below I will show some of the code work I did during this time. I will also include some pictures in this repository for viewing purposes.
</p>
<br>

<h2 style="color: blue;">Front End Stories</h2>

<h4>&middot; Make Uniform all Search Bars</h4>
<p>
A lot of the search bars on the website had different formatting. Four HTML files had search bars to which I added a new class called <i>.txtbox-margin</i> which I then targeted in the main CSS file allowing me and anyone else in the future to change the formatting of all the search bars from one location. Below is an example of the CSS code;
</p>
<p>CSS</p>
<pre>
.txtbox_margin {
    margin: 0px 0px 20px 0px;
}
</pre>
<br>
<hr>
<br>

<h4>&middot; Fix UL Styling for Dropdown Navigation</h4>
<p>
Someone had previous targeted the entire UL (unordered list) element within CSS changing the styling of all UL elements within the website when they intended it for only one section. I found and entered the correct HTML file, found the drop down nav and targeted the UL element with a class <i>.nav-center</i> to target in CSS. The code below reflects this.
</p>
<p>
CSS
</p>
<pre>
.nav-center {
    list-style-type: none;
    text-align: center;
}
</pre>
<br>
<hr>
<br>

<h4>&middot; Add a Video Background to the Front Page</h4>
<p>
Instead of a static image for the landing page, we wanted to change it to a video background that covers the page and is responsive to different screen sizes. Below is my code for the index HTML file and the main CSS file which I targeted with an ID <i>#bgVideo</i> since it is unique and will only be used once.
</p>
<p>
HTML
</p>
<pre>
&lt;video autoplay muted loop id=&quot;bgVideo&quot;&gt;&lt;source src=&quot;~/content/videos/NYC-Traffic.mp4&quot; /&gt;&lt;/video&gt;

</pre>

<p>
CSS
</p>
<pre>
#bgVideo {
    position: fixed;
    right: 0;
    bottom: 0;
    min-height: 100%;
    min-width: 100%;
    z-index: -1;
}
</pre>
<br>
<hr>