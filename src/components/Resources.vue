<template>
	<div class="resources-page">
		<div class="row" v-if="!user.isVolunteer">

	  	<div class="col-sm-12" style="background-color:rgba(255,208,115,.6); text-align:left; padding-left:50px;">
	  		<h3 style="color:white"><strong>Resources for Students</strong></h3>
	  	</div>
	    <div class = "row" style="text-align:left;padding-left:25px;padding-top:100px;">
	          <ul class=bigFont> Below are some sites that we think every student should be familiar with.</ul>
	    </div>
	       <div class="row">
	      	<div class = "col-sm-12" style="text-align:left;padding-left:50px;padding-bottom:40px">

	        	<h2 style="font-weight:bold">College Admissions Resources</h2>
	        	<br>
	        	<ul class=bigFont>
	        		<li><a href="https://collegereadiness.collegeboard.org/sat" target="_blank">SAT Website</a></li>
	        		<li><a href="http://www.act.org/content/act/en/students-and-parents.html" target="_blank">ACT Website</a></li>
	        		<li><a href="https://collegereadiness.collegeboard.org/sat-subject-tests" target="_blank">SAT Subject Tests</a></li>
	        		<li><a href="https://bigfuture.collegeboard.org/find-colleges" target="_blank">College Search Engine</a></li>
	        		<li><a href="http://www.commonapp.org/" target="_blank">The Common Application Website</a></li>
	        		<li><a href="https://www.commonapp.org/files/CommonAppRequirementsTracker.pdf" target="_blank">Application Requirements & Deadline Tracker</a></li>
	        		<li><a href="https://fafsa.ed.gov/" target="_blank">Free Application for Federal Student Aid (FAFSA)</a></li>
	        		<li><a href="https://student.collegeboard.org/css-financial-aid-profile" target="_blank">CSS/Financial Aid PROFILE</a></li>
	        		<li><a href="https://www.khanacademy.org/sat" target="_blank">SAT Practice Questions</a></li>
	        	</ul>
	        	<br>
	        	<h2 style="font-weight:bold">Math Resources</h2>
	        	<br>
	        	<ul class=bigFont>
	        	    <li><a href="https://www.khanacademy.org/math/" target="_blank">Khan Academy (math tutorial videos and practice questions)</a></li>
	        	    <li><a href="https://www.wolframalpha.com/" target="_blank">Online Calculator (can graph and solve equations)</a></li>
	        	    <li><a href="http://math.stackexchange.com/questions/tagged/calculus " target="_blank">Calculus Forum</a></li>
	        	</ul>
	       </div>
	    </div>
	    <br>
	    <p>Have ideas for additional resources to add to this page? Email <a>info@upchieve.org!</a></p>
	  </div>
		<div class="row" v-else>

	  	<div class="col-sm-12" style="background-color:rgba(255,208,115,.6); text-align:left; padding-left:50px;">
	  		<h3 style="color:white"><strong>Resources for Volunteers</strong></h3>
	  	</div>
	  	<div class = "row" style="text-align:left;padding-left:25px;padding-top:100px;">
	          <ul class=bigFont> Below are some links that you may need during your shift.</ul>
	    </div>
	       <div class="row">
	      	<div class = "col-sm-12" style="text-align:left;padding-left:50px;padding-bottom:40px">
	        	<ul class="bigFont">
	            <li><a href="https://drive.google.com/drive/folders/0B0I0kE7XX47FdG9oMXZQQWVhS2M?usp=sharing" target="_blank">Student Uploaded Files</a></li>
	            <li><a href="https://goo.gl/CfPZ2j" target="_blank">Most up to date volunteer schedule</a></li>
	            <li><a href="https://goo.gl/forms/RGwYN9nu6UbRVF713" target="_blank">Google Form to request schedule change</a></li>
	        		<li><a href="https://eliademy.com/app/a/courses/9296633213 " target="_blank">Math Tutor course on Eliademy</a></li>
	        		<li><a href="https://eliademy.com/app/a/courses/01af786cd6 " target="_blank">Admissions Consultant course on Eliademy</a></li>
	        		<li><a href="https://goo.gl/XfdE3X" target="_blank">Resources for Admissions Consultants</a></li>
	        	</ul>

	        </div>
	    </div>
	    <br>
	    <p>Have ideas for additional resources to add to this page? Email <a>info@upchieve.org!</a></p>
	  </div>
	</div>
</template>

<script>
import UserService from 'src/services/UserService';

export default {
	data(){
    return {
      user: UserService.getUser()
    }
  }
}
</script>

<style>
a:hover {

}

.bigFont li{
	 font-size: 20px;
}
</style>
