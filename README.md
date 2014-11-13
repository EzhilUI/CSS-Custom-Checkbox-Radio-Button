CSS-Custom-Checkbox-Radio-Button
================================

CSS Custom Check box / Radio Button with different Background image

<style>
/* CSS3- custom check box / Radio Button */
body{ font-family:Arial, Helvetica, sans-serif; font-size:15px; margin:30px;}
*{margin:0; padding:0;}

#wrapper{width:900px; margin:0 auto;}
.radioButton{float:left; width:50%;}
.checkbox{float:left; width:50%;}
.custom_ui span{ font-size:16px; margin:5px 0px 2px; float:left; width:100%;}

/*****Commoon css for checkbox/radio button******/
.custom_ui p{position:relative; margin: 6px 0px; width:100%; float:left; font-weight:bold;}
.custom_ui p > input{height: 16px;width: 16px;float:left;position: absolute;left: 0;opacity: 0;}
.custom_ui p > label{line-height: 16px;color: #fff;padding: 0 0 0 22px; font-weight:normal;	}

/*****Checkbox background-image css******/
.custom_ui p:not(#x) > input[type="checkbox"] + label{	background:url(images/checkbox.png) no-repeat;	height: 16px; color:#121212}
.custom_ui p:not(#foo) > input[type=checkbox]:checked + label{ background:url(images/checkbox_checked.png) no-repeat;; }
.checkbox label{padding-left:25px;}

/*****Radio button background-image css******/
.custom_ui p:not(#x) > input[type="radio"] + label{background:url(images/radio_uncheck.png) no-repeat;	height: 16px; color:#121212}
.custom_ui p:not(#x) > input[type=radio]:checked + label{background:url(images/radio_checked.png) no-repeat;}

</style>


<!---------Radio Button-------->
<div id="wrapper" class="custom_ui">
<div class="radioButton">
<h2> CSS3 Custom Radio Button</h2>
			<span>Gender:</span>
			<p><input type="radio"  id="male" name="gender" /> <label for="male">Male</label></p>
			<p><input type="radio"  id="female" name="gender" /> <label for="female">Female</label></p>
</div>

<!---------Checkbox-------->	

<div class="checkbox">
<h2> CSS3 Custom Checkbox</h2>	
			<span>Skills</span>
			
			<p><input type="checkbox"  id="HTML5"/> <label for="HTML5">HTML5</label></p>
			<p><input type="checkbox"  id="CSS3" /> <label for="CSS3">CSS3</label></p>
			<p><input type="checkbox"  id="Jquery"/> <label for="Jquery">Jquery</label></p>
			<p><input type="checkbox" id="AngularJS" /> <label for="AngularJS">Angular JS</label></p>
			</div>
	</div>
	
	
	
