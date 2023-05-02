Download Link: https://assignmentchef.com/product/solved-cop-2800-java-programming-project-4
<br>
5/5 - (1 vote)

 For this project, you will create a class called <code>TextKit</code> containing several utility methods that can be used in different applications.  This class is not intended to be a complete application by itself!  (It has no <code>main</code> method.)  Your class will be put into a package called <code>utils</code>.  The package will then be documented using the <code>javadoc</code> tool to create <abbr title="hyper-Text Markup Language">HTML</abbr> documentation for your package.  Finally, you will create a small stand-alone non-<abbr>GUI</abbr> Java program that tests the methods of your <code>utils.TextKit</code> class.

(Your next project will use this package, and you won’t be allowed to make any changes to <code>TextKit</code> once submitted.)

<h2>Requirements:</h2>

Create a public Java class named “<code>TextKit</code>” in a package called “<code>utils</code>” that contains the following <code>public static </code>methods (at least):

<ul>

 <li><code>lineOfStars</code>This method will create and return a <code>String</code> containing a line of asterisks (or stars).  This method <strong><big>must</big></strong> take a single parameter only, an <code>int</code> which says how many stars to draw.  For example, the code:System.out.println( utils.TextKit.lineOfStars(4) );Should print a line that looks like:****The intent is that <code>lineOfStars</code> should be a generally useful method that given a single number returns a <code>String</code> of that many stars.  (Such a method could easily be reused in another project someday.)</li>

 <li><code>pad</code>This method will format integers by adding spaces (called <dfn>padding</dfn>) to the left end, to make the resulting <code>String</code> a certain minimum length.  (If the number contains more digits than the specified width, then no padding is added.)  This method <strong><big>must</big></strong> take two <code>int</code> arguments, the first is the number to format, and the second is the desired minimum <code>String</code> length.  The resulting <code>String</code> is returned.  For example, the code:int num = 17; System.out.println( “*” + utils.TextKit.pad(num, 4) + “*” );Should print a line that looks like:* 17*(Notice there are two leading blanks added by <code>pad</code>, to make the field length 4.)</li>

</ul>

To facilitate such reuse, these methods <strong><big>must</big></strong> be <code>public static</code> methods of a public class called <code>TextKit</code>, which <strong><big>must</big></strong> be in a <code>package</code> called <code>utils</code>.  (Someday you might add other text utility methods to this class or add other classes to this package.)

Be sure to add appropriate <em>Java doc</em> comments throughout your code!

For full credit, your methods <strong>must</strong> check for invalid arguments (for example, inappropriate negative numbers).  If you detect invalid arguments passed to a method, the method must throw an appropriate <code>java.lang.IllegalArgumentException</code>.

Next, create a testing application.  Your test program (containing just a <code>main</code> method) should not be in the <code>utils</code> package, but rather in the default, nameless package.  You can name the class anything you like; something like <em>TextKitApp</em> is fine.  This test program should invoke each method of the <code>utils.TextKit</code> class at least once, to verify those methods work.  You can test the resulting <code>String</code>object returned from each method, against the expected value.  Or you can simply print a message that says something like “You should see five stars here: ”, followed by the output of the method call with (in this example) the argument <code>5</code>.  (Such a <code>main</code> method is sometimes referred to as a <dfn>test driver</dfn>.)  A good test driver will have many test cases, to more thoroughly check the methods.  Having failing cases (in a <code>try...catch</code> block of course) is also a good idea, but not required for this project.