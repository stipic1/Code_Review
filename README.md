# Live Project

<h3>Overview</h3>
<p>
The last two weeks of my time at the Tech Academy revolved around a live porject. Along with my peers we worked on fixing bugs, adding features, and updating the clients website. 
</p>

<p>We worked on a legacy code base which was begun by others before us. I worked on the front end (HTML, CSS, JavaScript) while others worked on the back end (C# & Python). Most of the CSS was done with vanilla CSS and Bootstrap. The software design pattern we used was MVC (Model-Viewer-Controller) which is what we will commonly see in the workplace. We used Microsoft Azure DevOps as our git repository and team workspace on the Visual Studio software. This taught me about the master branch vs other created branches, pulling, pushing, merging, and much more. We were able to assign ourselves 'stories' to complete for the project as is done in the software industry. We implemented the scrum method of sprints and daily stand-ups to keep everyone on the same page during the project. We were encouraged to treat this as a job and rely on one another through Slack or stand-ups if we needed help.
</p>

<p>
Below I will show some of the code work I did during this time. I will also include some pictures in this repository for viewing purposes.
</p>

<h3>Front End Stories</h3>
<br>

<h5>Make Uniform all Search Bars</h5>
<p>
A lot of the search bars on the website had different formatting. Four HTML files had search bars to which I added a new class called <i>.txtbox-margin</i> which I then targeted in the main CSS file allowing me and anyone else in the future to change the formatting of all the search bars from one location. Below is an example of the CSS code;
</p>
<quote>
<p>CSS</p>
.txtbox_margin {
    margin: 0px 0px 20px 0px;
}
</quote>
<br>

<h5>Fix UL Styling for Dropdown Navigation</h5>
<p>
Someone had previous targeted the entire UL (unordered list) element within CSS changing the styling of all UL elements within the website when they intended it for only one section. I found and entered the correct HTML file, found the drop down nav and targeted the UL element with a class <i>.nav-center</i> to target in CSS. The code below reflects this.
</p>
<p>
CSS
</p>
<quote>
.nav-center {
    list-style-type: none;
    text-align: center;
}
</quote>
<br>

<h5>Add a Video Background to the Front Page</h5>
<p>
Instead of a static image for the landing page, we wanted to change it to a video background that covers the page and is responsive to different screen sizes. Below is my code for the index HTML file and the main CSS file which I targeted with an ID since it is unique and will only be used once.
</p>
<p>
HTML
</p>
<quote>
<video autoplay muted loop id="bgVideo"><source src="~/content/videos/NYC-Traffic.mp4" /></video>

</quote>

<p>
CSS
</p>
<quote>
#bgVideo {
    position: fixed;
    right: 0;
    bottom: 0;
    min-height: 100%;
    min-width: 100%;
    z-index: -1;
}
</quote>