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
<pre><p>break;</p></pre>
<p>continue keyword will start loop from beginning</p>
<pre><p>continue;</p></pre>
<p>for each loop implementation</p>
<pre><p>for(dataType item : array) {}</p></pre>

<h2>Lists</h2>
<p>List Implementation</p>
<pre><p>java.util.ArrayList;<br/>
ArrayList<String> list = new ArrayList<>();</p></pre>
<p>Add item to list</p>
<pre><p>import java.util.ArrayList;</p>
<p>ArrayList<String> wordList = new ArrayList<>();</p>
<p>worList.add("first");</p></pre>
<p>get item from list</p>
<pre><p>// using example above</p>
<p>System.out.println(wordList.get(0));</p></pre>
<p>list size method</p>
<pre><p>list.size();</p></pre>
<p>list remove method</p>
<pre><p>list.remove();<br/>
// can also remove specific values
list.remove("remove same string value");<br/>
// can also remove int values using valueOf
list.remove(Integer.valueOf(15));</p></pre>
<p>list contains method</p>
<pre><p>list.contains();</p></pre>

<h2>Arrays</h2>
<p>method 1: create array</p>
<pre><p>int[] intArrayOf5Elements = new int[5];</p></pre>
<p>method 2: create array</p>
<pre><p>int[] intArrayOf5Elements = {1, 5, 3, 2, 0};</p></pre>
<p>length of array</p>
<pre><p>intArrayOf5Elements.length;</p></pre>

<h2>Strings</h2>
<p>split a string</p>
<pre><p>String myString = "text1 text2 text3";<br/>
String[] splitString = myString.split(" ");</p></pre>
<p>specific char in a string</p>
<pre><p>String text = "Hello World";<br/>
char character = text.charAt(0);</p></pre>
<p>Special note when using the length function for a string it requires length() compared to arrays</p>
<pre><p>example.length()</p></pre>

<h2>Classes</h2>
<p>Class template</p>
<pre><p>public class ClassName<br/>
{
<p>    // instance variables
    private String name;
    private int age;
</p>    
<p>    // constructor can also not specify anything for nothing
    public ClassName(String personName, int personAge)
    {
        this.name = personName;
        this.age = personAge;
    }
}</p></pre>

<h2Files and reading data</h2>
<p>reading from a file template</p>
<pre><p>import java.nio.file.Paths;</p>
<p>try(Scanner scanner = new Scanner(Paths.get("file.txt")));
{
    while(scanner.hasNextLine())
	{
		String row = scanner.nextLine();
		System.out.println(row);
	}
}</p>
<p>catch(Exception e)
{
    System.out.println("Error: " + e.getMessage());
}</pre>
