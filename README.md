<h1>Quick Java Syntax Reference</h1>
<h2>To compile and run Java code in Terminal</h2>
<ol>
	<li>To run single files</li>
	<ol type="1">
		<li>javac (program_name).java</li>
		<li>java (program_name)</li>
	</ol>
	<li>To run multiple files</li>
	<ol type="1">
		<li>javac (program_name_1).java (etc.).java (main_driver).java</li>
		<li>java (main_driver)</li>
	</ol>
</ol>

<h2>Print to console</h2>
<pre><code>System.out.println("insert print text");</code></pre>

<h2>User Input</h2>
<pre><p>import java.util.Scanner;<br/>
Scanner scanner = new Scanner(System.in);<br/>
String user_input = scanner.nextLine();
<p></pre>

<h2>Type Conversion</h2>
<p>Convert String to Int</p>
<pre><p>int user_input = Integer.valueOf(scanner.nextLine());</p></pre>
<p>Convert String to Double</p>
<pre><p>double user_input = Double.valueOf(scanner.nextLine());</p></pre>
<p>Convert String to Boolean</p>
<pre><p>boolean user_input = Boolean.valueOf(scanner.nextLine());</p></pre>

<h2>Type Casting</h2>
<p>change type of int to double</p>
<pre><p>double result = (double) 5 / 2;</p></pre>


<h2>comparison operator</h2>
<p>compare if a string equals another string</p>
<pre><p>String input = "test string";</p>
<p>if(input.equals("is it equal"))</p></pre>

<h2>Loops</h2>
<p>break keyword will exit loop</p>
<pre><p>break;</p>
<p>continue keyword will start loop from beginning</p>
<pre><p>continue;</p>
