# Laboratory-Activity-No.-06
Laboratory Activity No. 06: Web Forms


Instructions:
In this laboratory activity you are going to combine several of the form controls to make up a site registration form.

Step-By-Step Lab Activity Instructions:
To complete this laboratory activity, please complete all of the following requirements:
Create a new Transitional XHTML 1.0 document, with the skeleton in place. Then add a heading and introduction to what the user should be doing:
<?xml version="1.0" ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
 "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en"><head>
<head>
<title>Registration</title>
</head>
<body>
<h2>User Registration</h2>
<p>Please complete the following form to register with our site:</p>
</body>
</html>.


The form is going to be placed in a table with two columns so that the instructions are in the left column, and the form controls are aligned in the right column. (Without this, the form controls would look uneven across the page.) This is quite a common technique in writing forms. In the first two rows you can add text inputs for username and password, and then leave a row blank for spacing out the page:
<table>
<tr>
<td>User Name:</td>
<td><input type="text" name="txtUserName" size="20" /></td>
</tr>
<tr>
<td>Password:</td>
<td><input type="password" name="pwdPassword" size="20" /></td>
</tr>
<tr>
<td>&nbsp;</td>
<td>&nbsp;</td>
</tr>
</table> 


 After the username and the password, add two radio buttons for the user to indicate his or her gender:
<tr>
<td>Gender:</td>
<td><input type="radio" name="radSex" value="male" />Male</td>
</tr>
<tr>
<td></td>
<td><input type="radio" name="radSex" value="female" />Female</td>
</tr>
<tr><td>&nbsp;</td><td>&nbsp;</td></tr> 


Next you want to add a select box to indicate how the user heard about the web site: 
<tr>
<td>How did you hear about us?:</td>
<td>
<select name="selReferrer">
<option selected="selected" value="">Select answer</option>
<option value="website">Another website</option>
<option value="printAd">Magazine ad</option>
<option value="friend">From a friend</option>
<option value="other">Other</option>
</select>
</td>
</tr>
<tr><td>&nbsp;</td><td>&nbsp;</td></tr> 
 
 
 The last option for the user is whether they will subscribe to the newsletter on the site, which you accomplish with a checkbox. There is also the submit button for the form: 
<tr>
<td>Please select this box if you wish<br /> to be added to our mailing list
<br /><small>We will not pass on your details to any third
party.</small></td>
<td><input type="checkbox" name="chkMailingList" /></td>
</tr>
<tr>
<td></td>
<td><input type="submit" value="Register now" /></td>
</tr>
</table> 
