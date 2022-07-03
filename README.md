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
<pre><code>import java.util.Scanner;<br/>
Scanner scanner = new Scanner(System.in);<br/>
String user_input = scanner.nextLine();
</code></pre>
