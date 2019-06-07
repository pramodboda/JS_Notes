<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">var</span>  todo  <span class="token operator">=</span>  <span class="token punctuation">[</span><span class="token string">'HTML5'</span><span class="token punctuation">,</span>  <span class="token string">'CSS3'</span><span class="token punctuation">,</span>  <span class="token string">'JS'</span><span class="token punctuation">,</span>  <span class="token string">'ES6/ES7'</span><span class="token punctuation">,</span>  <span class="token string">'jQuery'</span><span class="token punctuation">,</span><span class="token string">'React'</span><span class="token punctuation">,</span>  <span class="token string">'TypeScript'</span><span class="token punctuation">,</span><span class="token string">'Angular'</span><span class="token punctuation">,</span>  <span class="token string">'Node'</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
</code></pre>
<h1 id="javascript-notes-by-pramod-boda">JavaScript Notes by Pramod Boda</h1>
<h2 id="core-javascript">Core JavaScript</h2>
<ol>
<li>
<p>Introduction</p>
</li>
<li>
<p>Lexical Structure</p>
<ul>
<li>Character Set</li>
<li>Comments</li>
<li>Literals</li>
<li>Identifiers</li>
<li>Reserved Words</li>
</ul>
</li>
<li>
<p>Types</p>
<ul>
<li><code>Numbers</code></li>
<li><code>String</code>(Text)</li>
<li><code>Boolean</code> Values</li>
<li><code>null</code></li>
<li><code>undefined</code></li>
<li><code>Object</code></li>
</ul>
</li>
<li>
<p>Variables</p>
<ul>
<li>Variable Declaration</li>
<li>Variable Scope</li>
</ul>
</li>
<li>
<p>Expressions</p>
</li>
<li>
<p>Operators</p>
<ul>
<li>Assignment Operators</li>
<li>Comparison Operators</li>
<li>Arithmetic Operators</li>
<li>Bitwise Operators</li>
<li>Logical Operators</li>
<li>String Operators</li>
<li>Conditional Operators</li>
<li>Comma Operators</li>
<li>Unary Operators</li>
<li>Relational Operators</li>
</ul>
</li>
<li>
<p>Statements</p>
<ul>
<li>
<p>Expresstion Statements</p>
</li>
<li>
<p>Compound &amp; Empty Statements</p>
</li>
<li>
<p>Declaration Statements</p>
</li>
<li>
<p>Conditional Statements</p>
<ul>
<li><code>if</code></li>
<li><code>else if</code></li>
<li><code>switch</code></li>
</ul>
</li>
<li>
<p>Loop Statements</p>
<ul>
<li>while</li>
<li>do/while</li>
<li>for</li>
<li>for in</li>
</ul>
</li>
<li>
<p>Jumps</p>
<ul>
<li>Labeled Statements</li>
<li><code>break</code></li>
<li><code>continue</code></li>
<li><code>return</code></li>
<li><code>throw</code></li>
<li><code>try</code> / <code>catch</code> / <code>finally</code></li>
</ul>
</li>
<li>
<p>Miscellaneous Statements</p>
<ul>
<li><code>with</code></li>
<li><code>debugger</code></li>
<li><code>"use strict"</code></li>
</ul>
</li>
<li>
<p>Summary of JavaScript Statements</p>
</li>
</ul>
</li>
<li>
<p>Objects</p>
</li>
<li>
<p>Arrays</p>
</li>
<li>
<p>Functions</p>
</li>
<li>
<p>Class &amp; Modules</p>
</li>
<li>
<p>Pattern Matching with Regular Expressions</p>
</li>
</ol>
<p><a id="jsIntroduction"></a></p>
<h2 id="introduction">Introduction</h2>
<h3 id="what-is-javascript">What is JavaScript?</h3>
<ul>
<li>JavaScript is the Programming language of the <strong>Web</strong></li>
<li>JavaScript is part of the triad of technologies that all developers must learn</li>
</ul>

<table>
<thead>
<tr>
<th>Language</th>
<th>Role</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>HTML</td>
<td>Content</td>
<td>to specify the content of the web pages.</td>
</tr>
<tr>
<td>CSS</td>
<td>Presentation</td>
<td>to specify the presentation of the web pages.</td>
</tr>
<tr>
<td>JS</td>
<td>Behavior</td>
<td>to specify the behavior of the web pages.</td>
</tr>
</tbody>
</table><ul>
<li>
<p>JavaScript is a high-level programming language.</p>
</li>
<li>
<p>JavaScript is a case-sensitive language.</p>
<ul>
<li>
<p>This means that language <code>keywords</code>, <code>variables</code>, <code>function</code> names, and other <code>identifiers</code> must always be typed with a consistent capitalization of letters.</p>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token keyword">var</span> name <span class="token operator">=</span> <span class="token string">"Pramod Boda"</span><span class="token punctuation">;</span> <span class="token comment">//initiated variable 'name'</span>
 Name<span class="token punctuation">;</span> <span class="token comment">// will not be same as 'name'</span>
 NAME<span class="token punctuation">;</span> <span class="token comment">// will not be same as 'name'</span>
 name<span class="token punctuation">;</span> <span class="token operator">=&gt;</span> <span class="token string">"Pramod Boda"</span>
</code></pre>
</li>
</ul>
</li>
<li>
<p>All web browsers support it without the need for plug-ind by means of a built-in JavaScript engine.</p>
</li>
<li>
<p>JavaScript is used on desktops, games consoles, tablets, and smart phones.</p>
</li>
<li>
<p>Including JavaScript interpreters, making JavaScript the most ubiquitous programming language in history.</p>
</li>
<li>
<p>JavaScript well-suited to object-oriented and functional programming style.</p>
</li>
<li>
<p>The overwhelming majority of modern websites use JavaScript, and all web browsers.</p>
</li>
<li>
<p>JavaScript has long since out grown its scripting - language roots to become a robust and efficient general - purpose language.</p>
</li>
</ul>
<p><a href="#toc"><img src="images/toc.png" width="24" height="24"></a></p>
<p><a id="jsLexicalStructure"></a></p>
<h2 id="lexical-structure">Lexical Structure</h2>
<ul>
<li>The lexical structure of a programming language is the set of elementary rules that specifies how you write programs in that language.</li>
</ul>
<h3 id="character-set">Character Set</h3>
<ul>
<li>JavaScript programs are writing using the Unicode character set.</li>
<li>Unicode is a superset of ASCII and Latin-1 and supports virtually every written language currently used on the planet.</li>
</ul>
<h3 id="case-sensitivity">Case sensitivity</h3>
<ul>
<li>JavaScript is a case-sensitive language. This means that language <code>keywords</code>, <code>variables</code>, <code>function</code> names, and other <code>identifies</code> must always be typed with consistent capitalization of letters.</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token keyword">var</span> name <span class="token operator">=</span> <span class="token string">"Pramod Boda"</span><span class="token punctuation">;</span> <span class="token comment">//initiated variable 'name'</span>
 Name<span class="token punctuation">;</span> <span class="token comment">// will not be same as 'name'</span>
 NAME<span class="token punctuation">;</span> <span class="token comment">// will not be same as 'name'</span>
 name<span class="token punctuation">;</span> <span class="token operator">=&gt;</span> <span class="token string">"Pramod Boda"</span>
</code></pre>
<blockquote>
<p>Note: however, thet HTML is not case-sensitive(althought XHTML is).</p>
</blockquote>
<ul>
<li>Many client-side JavaScript objects and properties have the same names as the HTML tags and attributes they represent.</li>
<li>While these tags and attributes names can be typed in any case in HTML, In JavaScript they typically must be all lowercase.</li>
</ul>
<blockquote>
<p>The HTML onclick event handler attribute is sometimes specified as onClick in HTML, but it must be specified as onclick in JavaScript code(or in XHTML documents).</p>
</blockquote>
<h3 id="comments">Comments</h3>
<ul>
<li>JavaScript supports two style of comments.</li>
<li>Any text between a // and the end of a line is treated as a comment. and is ignored by JavaScript.</li>
<li>Single comment example:</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token comment">// This is a Single line comment.</span>
</code></pre>
<ul>
<li>Any text between the characters /* and */ is also treated as a comment; These comments may span mutiple lines but may not be nested.</li>
<li>Multi-Line comment example:</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token comment">/* 
 * This is a
 * Multiple lines
 * comment.
 */</span>
</code></pre>
<h3 id="literals">Literals</h3>
<ul>
<li>A literals is a data that appears directly in a program.</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token number">46</span> <span class="token comment">// The Number forty six.</span>
 <span class="token number">4.6</span> <span class="token comment">// The Number four point six.</span>
 <span class="token string">"Hylo World"</span> <span class="token comment">// A String of text.</span>
 <span class="token string">'Hi'</span> <span class="token comment">// Another String.</span>
 <span class="token boolean">true</span> <span class="token comment">// A Boolean value.</span>
 <span class="token boolean">false</span> <span class="token comment">// another Booleans value.</span>
 <span class="token operator">/</span>javascript<span class="token operator">/</span>gi <span class="token comment">// A regular expression literal (for pattern matching)</span>
 <span class="token keyword">null</span> <span class="token comment">// Absence of object.</span>
</code></pre>
<pre class=" language-javascript"><code class="prism  language-javascript"> x<span class="token punctuation">:</span><span class="token number">3</span><span class="token punctuation">,</span> y<span class="token punctuation">:</span><span class="token number">5</span> <span class="token comment">// An object initializer</span>
 <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">,</span>a<span class="token punctuation">,</span>b<span class="token punctuation">,</span>c<span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">]</span> <span class="token comment">// An array initializer.</span>
</code></pre>
<h3 id="identifiers">Identifiers</h3>
<ul>
<li>An identifires is simple a name. In JavaScript, identifires are used to name variables and functions and to provide labels for certain loops in JavaScript code.</li>
<li>These are all legal identifiers:</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token keyword">var</span> trueVar <span class="token comment">// variable initialization</span>
 <span class="token function">my_variable_name</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token comment">// function name</span>
 <span class="token keyword">var</span> v143 <span class="token comment">// variable initialization</span>
 <span class="token function">_trueVariable</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token comment">// function name</span>
 <span class="token keyword">var</span> $strVariable <span class="token comment">// variable initialization</span>
</code></pre>
<h4 id="mathematical-symbols">Mathematical symbols</h4>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token keyword">var</span> si <span class="token operator">=</span> <span class="token boolean">true</span><span class="token punctuation">;</span>
 <span class="token keyword">var</span> π <span class="token operator">=</span> <span class="token number">3.14</span><span class="token punctuation">;</span>
</code></pre>
<h3 id="reserved-words">Reserved Words</h3>
<ul>
<li>You cannot use these words as <code>identifiers</code> in your programs.</li>
</ul>

<table>
<thead>
<tr>
<th>*</th>
<th>*</th>
<th>*</th>
<th>*</th>
<th>*</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>break</code></td>
<td><code>delete</code></td>
<td><code>function</code></td>
<td><code>return</code></td>
<td><code>typeof</code></td>
</tr>
<tr>
<td><code>case</code></td>
<td><code>do</code></td>
<td><code>if</code></td>
<td><code>switch</code></td>
<td><code>var</code></td>
</tr>
<tr>
<td><code>catch</code></td>
<td><code>else</code></td>
<td><code>in</code></td>
<td><code>this</code></td>
<td><code>void</code></td>
</tr>
<tr>
<td><code>continue</code></td>
<td><code>false</code></td>
<td><code>instanceof</code></td>
<td><code>throw</code></td>
<td><code>while</code></td>
</tr>
<tr>
<td><code>debugger</code></td>
<td><code>finally</code></td>
<td><code>new</code></td>
<td><code>true</code></td>
<td><code>with</code></td>
</tr>
<tr>
<td><code>default</code></td>
<td><code>for</code></td>
<td><code>null</code></td>
<td><code>try</code></td>
<td></td>
</tr>
</tbody>
</table><p><strong>Non-reserved words that act like reserved words</strong></p>
<ul>
<li>The <code>NaN</code>, <code>Infinity</code>, <code>undefined</code> properties of the global ogject are immutable or read-only properties in ES5. So even though <code>var NaN = 42;</code> in the global scope wouldn’t throw an error, it wouldn’t actually do anything</li>
<li>To avoid confusion, I’d suggest you to avoiding the use of these <code>variable</code> names.</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"> <span class="token comment">//In the global scope</span>
 <span class="token keyword">var</span> <span class="token number">NaN</span> <span class="token operator">=</span> <span class="token number">42</span><span class="token punctuation">;</span>
 console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token number">NaN</span><span class="token punctuation">)</span><span class="token punctuation">;</span> <span class="token comment">// NaN</span>
 
 <span class="token comment">//...but elsewhere</span>
 <span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">{</span>
	 <span class="token keyword">var</span> <span class="token number">NaN</span> <span class="token operator">=</span> <span class="token number">42</span><span class="token punctuation">;</span>
	 console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token number">NaN</span><span class="token punctuation">)</span><span class="token punctuation">;</span> <span class="token comment">// 42</span>
 <span class="token punctuation">}</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<h3 id="dynamic-typing">Dynamic Typing</h3>
<p>JavaScript is a loosely typed or a dynamic language.</p>
<h2 id="statements">Statements</h2>
<ul>
<li><code>Statements</code> are JavaScript sentences or commands.</li>
<li>Just as English sentences are terminated and separated from each other with periods, JavaScript statements are terminated with semicolons.</li>
<li><code>Expressions</code> are <em>evaluated</em> to produce a <code>value</code>, but <code>statements</code> are <em>executed</em> to make something happen.</li>
</ul>
<h2 id="arrays">9. Arrays</h2>
<h3 id="list-of-array-properties">List of Array properties</h3>
<ul>
<li>constructor</li>
<li>length</li>
<li>prototype</li>
</ul>
<h3 id="list-of-array-methods">List of Array methods</h3>
<ul>
<li>
<h3 id="manipulating-arrays-with-methods---to-add-or-remove-elements">Manipulating Arrays with Methods - To Add or Remove elements</h3>
<ul>
<li><code>push(...items)</code> - adds item to the end.</li>
<li><code>unshift(...items)</code> - adds item from the beginning.</li>
<li><code>pop()</code> - extracts/ removes an item from the end.</li>
<li><code>shift()</code> - extracts/ removes an item from the beginning.</li>
<li><code>splice(pos, deleteCount, ...items)</code> - at index <code>pos</code> delete <code>deleteCount</code> elements and insert <code>items</code>.</li>
</ul>
</li>
</ul>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">var</span>  todo  <span class="token operator">=</span>  <span class="token punctuation">[</span><span class="token string">'HTML5'</span><span class="token punctuation">,</span>  <span class="token string">'CSS3'</span><span class="token punctuation">,</span>  <span class="token string">'JS'</span><span class="token punctuation">,</span>  <span class="token string">'ES6/ES7'</span><span class="token punctuation">,</span>  <span class="token string">'jQuery'</span><span class="token punctuation">,</span><span class="token string">'React'</span><span class="token punctuation">,</span>  <span class="token string">'TypeScript'</span><span class="token punctuation">,</span><span class="token string">'Angular'</span><span class="token punctuation">,</span>  <span class="token string">'Node'</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
</code></pre>
<p>Add element to the end.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">	todo<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token string">'Less'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span> <span class="token operator">+</span> todo<span class="token punctuation">.</span>length <span class="token operator">+</span> <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<p>Add element from the beginning.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">todo<span class="token punctuation">.</span><span class="token function">unshift</span><span class="token punctuation">(</span><span class="token string">'Semantic UI'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span> <span class="token operator">+</span> todo<span class="token punctuation">.</span>length <span class="token operator">+</span> <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<p>Remove element from the end.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">todo<span class="token punctuation">.</span><span class="token function">pop</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span> <span class="token operator">+</span> todo<span class="token punctuation">.</span>length <span class="token operator">+</span> <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<p>Remove element from the beginning.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">todo<span class="token punctuation">.</span><span class="token function">shift</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span> <span class="token operator">+</span> todo<span class="token punctuation">.</span>length <span class="token operator">+</span> <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<p>Not deleting any element from the array, But just adding a element to array.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">todo<span class="token punctuation">.</span><span class="token function">splice</span><span class="token punctuation">(</span><span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token string">'Bootstrap'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span>  <span class="token operator">+</span>  todo<span class="token punctuation">.</span>length  <span class="token operator">+</span><span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token comment">//Output =&gt; You have 10 todos</span>
<span class="token comment">//Output =&gt; (10) ["HTML5", "CSS3", "JS", "Bootstrap", "ES6/ES7", "jQuery", "React", "TypeScript", "Angular", "Node"]</span>
</code></pre>
<p>Now we want to delete the element and replace the element in the same place.</p>
<pre class=" language-javascript"><code class="prism  language-javascript">todo<span class="token punctuation">.</span><span class="token function">splice</span><span class="token punctuation">(</span><span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token string">'ES6+'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span>  <span class="token operator">+</span>  todo<span class="token punctuation">.</span>length  <span class="token operator">+</span><span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>todo<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token comment">//Output =&gt; You have 10 todos</span>
<span class="token comment">//Output =&gt; (10) ["HTML5", "CSS3", "JS", "Bootstrap", "ES6+", "jQuery", "React", "TypeScript", "Angular", "Node"]</span>
</code></pre>
<h3 id="looping-over-array">Looping over Array</h3>
<p><strong><code>forEach(Func)</code></strong> - Calls <code>func</code> for every element, does not return anything.</p>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">const</span>  todo2  <span class="token operator">=</span>  <span class="token punctuation">[</span><span class="token string">'Make Art'</span><span class="token punctuation">,</span><span class="token string">'Develop Website'</span><span class="token punctuation">,</span><span class="token string">'Learn Web Development'</span><span class="token punctuation">,</span>  <span class="token string">'Do Exercises'</span><span class="token punctuation">,</span>  <span class="token string">'Earn Money'</span><span class="token punctuation">,</span><span class="token string">'Save Money'</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span>  <span class="token operator">+</span>todo2<span class="token punctuation">.</span>length<span class="token operator">+</span>  <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
todo2<span class="token punctuation">.</span><span class="token function">forEach</span><span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span>item<span class="token punctuation">,</span> index<span class="token punctuation">)</span><span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>index<span class="token operator">+</span><span class="token string">' : '</span><span class="token operator">+</span>item<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token comment">// Now we will little extened our code for perfect numbering display.</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">'You have '</span>  <span class="token operator">+</span>todo2<span class="token punctuation">.</span>length<span class="token operator">+</span>  <span class="token string">' todos'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
todo2<span class="token punctuation">.</span><span class="token function">forEach</span><span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span>todo2<span class="token punctuation">,</span> index<span class="token punctuation">)</span><span class="token punctuation">{</span>
	<span class="token keyword">var</span>  numInc  <span class="token operator">=</span>  index <span class="token operator">+</span> <span class="token number">1</span><span class="token punctuation">;</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>numInc<span class="token operator">+</span><span class="token string">' : '</span><span class="token operator">+</span>todo2<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<pre><code>	-  `concat(...items)` - Joins two or more arrays, and returns a copy of the joined arrays

	-  `copyWithin()` - Copies array elements within the array, to and from specified positions.
		&gt; Note: The `copyWithin()` method is not supported in IE 11 (and earlier versions).

	-  `every()` - checks if every element in an array pass a test.

	-  `fill()` - Fill the elements in an array with a static value.

	&gt; Note: The `fill()` method is not supported in IE 11 (and earlier versions).

	-  `filter()` - Creates a new array with every element in an array that pass a test.

	&gt; Note: The `filter()` method is not supported in IE 11 (and earlier versions).

	-  `find()` - Returns the value of the first element in an array that pass a test.

	&gt; Note: The `find()` method is not supported in IE 11 (and earlier versions).

	-  `findIndex()` - Returns the index of the first element in an array that pass a test. `findIndex()` is like `find()`, but returns the index instead of a value.

	&gt; Note: The `findIndex()` method is not supported in IE 11 (and earlier versions).
</code></pre>
<ul>
<li>
<p>To iterate over elements:</p>
</li>
<li>
<p><code>forEach(func)</code> - Calls a function for each array element, does not return anything.</p>
</li>
<li>
<p>To transform the array:</p>
</li>
<li>
<p><code>map(func)</code> - creates a new array from result of calling <code>func</code> for every element.</p>
</li>
<li>
<p><code>sort(func)</code> - sorts the array in-place, then returns it.</p>
</li>
<li>
<p><code>reverse()</code> - reverses the array in-place, then returns it.</p>
</li>
<li>
<p><code>split/join</code> - convert a string to array and back.</p>
</li>
<li>
<p><code>reduce(func, initial)</code> - calculate a single value over the array by calling <code>func</code> for each element and passing an intermediate result between the calls.</p>
</li>
</ul>

