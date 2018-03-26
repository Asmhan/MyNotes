---


---

<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">print</span> <span class="token string">'shanioob'</span> <span class="token operator">+</span> <span class="token number">5</span><span class="token operator">/</span><span class="token number">2</span>	<span class="token comment">#will produce an error</span>
<span class="token comment">#TypeError: unsupported operand type(s) for /: 'str' and 'int'</span>
<span class="token keyword">print</span> <span class="token string">'shanioob'</span> <span class="token operator">*</span> <span class="token number">5</span><span class="token operator">/</span><span class="token number">2</span>	<span class="token comment">#will produce an error</span>
<span class="token keyword">print</span> <span class="token string">'shanioob'</span> <span class="token operator">*</span> <span class="token punctuation">(</span><span class="token number">5</span><span class="token operator">/</span><span class="token number">2</span><span class="token punctuation">)</span>	<span class="token comment">#will produce 'shanioobshanioob'</span>
<span class="token keyword">print</span>          <span class="token number">5</span><span class="token operator">/</span><span class="token number">2.0</span>
</code></pre>
<h2 id="strings">Strings</h2>
<pre class=" language-python"><code class="prism  language-python">the_king <span class="token operator">=</span> <span class="token string">"the king"</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">'t'</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span> <span class="token operator">+</span> the_king<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">"th"</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">:</span><span class="token number">2</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">"th"</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">:</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">"he king"</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token number">2</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">"th"</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token operator">-</span><span class="token number">1</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token string">"the kin"</span>

the_king<span class="token punctuation">.</span>find<span class="token punctuation">(</span><span class="token string">'king'</span><span class="token punctuation">)</span>
the_king<span class="token punctuation">.</span>find<span class="token punctuation">(</span><span class="token string">'king'</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span>
the_king<span class="token punctuation">.</span>replace<span class="token punctuation">(</span><span class="token string">'king'</span><span class="token punctuation">,</span> <span class="token string">'queen'</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">)</span>
<span class="token keyword">assert</span> the_king<span class="token punctuation">.</span>split<span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token punctuation">[</span><span class="token string">"the"</span><span class="token punctuation">,</span> <span class="token string">"king"</span><span class="token punctuation">]</span>
</code></pre>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">assert</span> <span class="token builtin">type</span><span class="token punctuation">(</span>shanioob_the_king<span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token string">"&lt;class ‘string’&gt;"</span>
<span class="token builtin">dir</span><span class="token punctuation">(</span><span class="token punctuation">)</span>
<span class="token builtin">dir</span><span class="token punctuation">(</span><span class="token string">'__builtins__'</span><span class="token punctuation">)</span>
<span class="token builtin">help</span><span class="token punctuation">(</span><span class="token string">'modules'</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="string-templates">String Templates</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token string">"{}- I am the number {} programmer"</span><span class="token punctuation">.</span><span class="token builtin">format</span><span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="coercion">Coercion</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">assert</span> <span class="token builtin">bool</span><span class="token punctuation">(</span><span class="token number">28</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token boolean">True</span>
<span class="token keyword">assert</span> <span class="token builtin">str</span><span class="token punctuation">(</span><span class="token boolean">True</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token string">'True'</span>
<span class="token keyword">assert</span> <span class="token builtin">int</span><span class="token punctuation">(</span><span class="token boolean">False</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token number">0</span>
</code></pre>
<h2 id="functions">functions</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">say_hello</span><span class="token punctuation">(</span>name<span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token keyword">return</span> <span class="token string">'Hello '</span> <span class="token operator">+</span> <span class="token builtin">str</span><span class="token punctuation">(</span>name<span class="token punctuation">)</span> <span class="token operator">+</span> <span class="token string">'!'</span> 
	
<span class="token keyword">print</span> say_hello<span class="token punctuation">(</span><span class="token string">'Susan'</span><span class="token punctuation">)</span>

five<span class="token punctuation">,</span> seven <span class="token operator">=</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span>
fiveSeven <span class="token operator">=</span> <span class="token punctuation">[</span>five<span class="token punctuation">,</span> seven<span class="token punctuation">]</span>

<span class="token keyword">def</span> <span class="token function">sum</span><span class="token punctuation">(</span>a<span class="token punctuation">,</span> b<span class="token punctuation">)</span><span class="token punctuation">:</span>
    a <span class="token operator">=</span> a <span class="token operator">+</span> b
<span class="token builtin">sum</span><span class="token punctuation">(</span>five<span class="token punctuation">,</span> seven<span class="token punctuation">)</span>	<span class="token comment">#five still == 5</span>

<span class="token keyword">def</span> <span class="token function">summer</span><span class="token punctuation">(</span><span class="token builtin">list</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token builtin">list</span><span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span> <span class="token operator">+</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span>
summer<span class="token punctuation">(</span>fiveSeven<span class="token punctuation">)</span>	<span class="token comment">#fiveSeven == [12, 7]</span>
</code></pre>
<h3 id="functions-default-arguments">Function’s Default Arguments</h3>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">cm</span><span class="token punctuation">(</span>feet <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">,</span> inches <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	inches_to_cm <span class="token operator">=</span> inches <span class="token operator">*</span> <span class="token number">2.54</span>
	feet_to_cm <span class="token operator">=</span> feet <span class="token operator">*</span> <span class="token number">12</span> <span class="token operator">*</span> <span class="token number">2.54</span>
	<span class="token keyword">return</span> inches_to_cm <span class="token operator">+</span> feet_to_cm

cm<span class="token punctuation">(</span>inches <span class="token operator">=</span> <span class="token number">70</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="if-statement--ternary-operator">if Statement &amp; Ternary Operator</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token function">bigger</span><span class="token punctuation">(</span>a<span class="token punctuation">,</span> b<span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token keyword">if</span> a <span class="token operator">&gt;</span> b<span class="token punctuation">:</span>
		<span class="token keyword">return</span> a
	<span class="token keyword">elif</span> b <span class="token operator">&gt;</span> a<span class="token punctuation">:</span>
		<span class="token keyword">return</span> b
	<span class="token keyword">else</span><span class="token punctuation">:</span>
		<span class="token keyword">return</span> a

<span class="token keyword">def</span> <span class="token function">bigger</span><span class="token punctuation">(</span>a<span class="token punctuation">,</span> b<span class="token punctuation">)</span><span class="token punctuation">:</span>
    <span class="token keyword">return</span> a <span class="token keyword">if</span> a <span class="token operator">&gt;</span> b <span class="token keyword">else</span> b
</code></pre>
<h2 id="logic-operators">Logic Operators</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token boolean">True</span> <span class="token operator">or</span> <span class="token boolean">False</span>
<span class="token boolean">True</span> <span class="token operator">and</span> <span class="token boolean">False</span>
<span class="token operator">not</span> <span class="token boolean">True</span> <span class="token operator">and</span> <span class="token operator">not</span> <span class="token boolean">False</span>
<span class="token operator">not</span> <span class="token boolean">True</span> <span class="token operator">!=</span> <span class="token boolean">None</span>
</code></pre>
<h2 id="while-loops">While Loops</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">while</span> <span class="token boolean">True</span><span class="token punctuation">:</span>
	<span class="token builtin">sum</span> <span class="token operator">+=</span> <span class="token number">1</span>	<span class="token comment">#the ++ syntax is not supported</span>
</code></pre>
<h2 id="for-loops">For Loops</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">for</span> num <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token comment">#do that 10 times</span>
</code></pre>
<h2 id="lists">Lists</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token builtin">list</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">,</span><span class="token punctuation">[</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">]</span><span class="token punctuation">]</span>
<span class="token keyword">assert</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token number">2</span>
<span class="token keyword">assert</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token number">2</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">]</span>
<span class="token keyword">assert</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token number">3</span><span class="token punctuation">]</span> <span class="token operator">+</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token number">3</span><span class="token punctuation">]</span> <span class="token operator">==</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">]</span>

<span class="token builtin">list</span> <span class="token operator">=</span> <span class="token builtin">list</span> <span class="token operator">+</span> <span class="token punctuation">[</span><span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">]</span>	<span class="token comment">#will create a new array</span>
<span class="token builtin">list</span><span class="token punctuation">.</span>append<span class="token punctuation">(</span><span class="token number">6</span><span class="token punctuation">)</span>			<span class="token comment">#will mutate the actual array</span>
<span class="token builtin">list</span> <span class="token operator">+=</span> <span class="token punctuation">[</span><span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">]</span>			<span class="token comment">#will mutate the actual array</span>

<span class="token keyword">assert</span> <span class="token builtin">list</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token number">2</span><span class="token punctuation">]</span> <span class="token operator">*</span> <span class="token number">2</span> <span class="token operator">==</span> <span class="token punctuation">[</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span> <span class="token punctuation">]</span>

<span class="token keyword">assert</span> <span class="token builtin">len</span><span class="token punctuation">(</span><span class="token builtin">list</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token number">4</span>
<span class="token keyword">assert</span> <span class="token builtin">len</span><span class="token punctuation">(</span><span class="token string">"My list"</span><span class="token punctuation">)</span> <span class="token operator">==</span> <span class="token number">7</span>

<span class="token builtin">list</span><span class="token punctuation">.</span>index<span class="token punctuation">(</span><span class="token number">6</span><span class="token punctuation">)</span>	<span class="token comment">#return index or error</span>
<span class="token number">6</span> <span class="token keyword">in</span> <span class="token builtin">list</span> 	<span class="token comment">#return True or False</span>
<span class="token operator">not</span> <span class="token number">6</span> <span class="token keyword">in</span> <span class="token builtin">list</span> <span class="token operator">==</span> <span class="token number">6</span> <span class="token operator">not</span> <span class="token keyword">in</span> <span class="token builtin">list</span>

<span class="token string">" "</span><span class="token punctuation">.</span>join<span class="token punctuation">(</span><span class="token builtin">list</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="tuples">Tuples</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token builtin">tuple</span> <span class="token operator">=</span> <span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span>
<span class="token punctuation">(</span>one<span class="token punctuation">,</span> two<span class="token punctuation">,</span> three<span class="token punctuation">)</span> <span class="token operator">=</span> <span class="token builtin">tuple</span>

one<span class="token punctuation">,</span> two<span class="token punctuation">,</span> three <span class="token operator">=</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">3</span>	<span class="token comment">#valid syntax</span>
</code></pre>
<h2 id="assertion--error-handling">Assertion &amp; Error Handling</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">try</span><span class="token punctuation">:</span>
	<span class="token keyword">assert</span> isDefined<span class="token punctuation">(</span>arg1<span class="token punctuation">)</span>
<span class="token keyword">except</span> AssertionError<span class="token punctuation">:</span>
	<span class="token keyword">print</span> <span class="token string">"AssertionError raised"</span>
</code></pre>
<h2 id="user-input">User Input</h2>
<pre class=" language-python"><code class="prism  language-python">user_input <span class="token operator">=</span> <span class="token builtin">raw_input</span><span class="token punctuation">(</span><span class="token string">"Type your input: "</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="used-import-statement">Used Import Statement</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">from</span> random <span class="token keyword">import</span> randint
random <span class="token operator">=</span> randint<span class="token punctuation">(</span><span class="token number">0</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">)</span>

<span class="token keyword">import</span> random
random <span class="token operator">=</span> random<span class="token punctuation">.</span>randint<span class="token punctuation">(</span><span class="token number">0</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">)</span>

<span class="token keyword">import</span> webbrowser
webbrowser<span class="token punctuation">.</span><span class="token builtin">open</span><span class="token punctuation">(</span><span class="token string">"https://www.google.com"</span><span class="token punctuation">)</span>

<span class="token keyword">import</span> time
time<span class="token punctuation">.</span>sleep<span class="token punctuation">(</span><span class="token number">60</span><span class="token punctuation">)</span>		<span class="token comment">#time is seconds</span>
this_time <span class="token operator">=</span> time<span class="token punctuation">.</span>ctime<span class="token punctuation">(</span><span class="token punctuation">)</span>

<span class="token keyword">import</span> os
os<span class="token punctuation">.</span>listdir<span class="token punctuation">(</span>r<span class="token string">"c:\OOP\prank"</span><span class="token punctuation">)</span>
os<span class="token punctuation">.</span>rename<span class="token punctuation">(</span>src<span class="token punctuation">,</span> dst<span class="token punctuation">)</span>
os<span class="token punctuation">.</span>getcwd<span class="token punctuation">(</span><span class="token punctuation">)</span>
os<span class="token punctuation">.</span>chdir<span class="token punctuation">(</span>path<span class="token punctuation">)</span>

string<span class="token punctuation">.</span>translate<span class="token punctuation">(</span>s<span class="token punctuation">,</span> table<span class="token punctuation">[</span><span class="token punctuation">,</span> deletechars<span class="token punctuation">]</span><span class="token punctuation">)</span>
string<span class="token punctuation">.</span>translate<span class="token punctuation">(</span><span class="token boolean">None</span><span class="token punctuation">,</span> <span class="token string">"0123456789"</span><span class="token punctuation">)</span>
</code></pre>
<h3 id="turtle-class">turtle class</h3>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">import</span> turtle

window <span class="token operator">=</span> turtle<span class="token punctuation">.</span>Screen<span class="token punctuation">(</span><span class="token punctuation">)</span>
window<span class="token punctuation">.</span>bgcolor<span class="token punctuation">(</span><span class="token string">"red"</span> <span class="token operator">or</span> <span class="token number">255</span><span class="token punctuation">,</span><span class="token number">255</span><span class="token punctuation">,</span><span class="token number">255</span> <span class="token operator">or</span> <span class="token string">"#rrggbb"</span><span class="token punctuation">)</span>

my_turtle <span class="token operator">=</span> turtle<span class="token punctuation">.</span>Turtle<span class="token punctuation">(</span><span class="token punctuation">)</span> 
	<span class="token operator">or</span> turtle<span class="token punctuation">.</span>Pen<span class="token punctuation">(</span><span class="token punctuation">)</span>

my_turtle<span class="token punctuation">.</span>forward<span class="token punctuation">(</span>distance<span class="token punctuation">)</span> 
	<span class="token operator">or</span> fd<span class="token punctuation">(</span>distance<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>backward<span class="token punctuation">(</span>distance<span class="token punctuation">)</span> 
	<span class="token operator">or</span> bk<span class="token punctuation">(</span>distance<span class="token punctuation">)</span> 
	<span class="token operator">or</span> back<span class="token punctuation">(</span>distance<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>right<span class="token punctuation">(</span>degrees<span class="token punctuation">)</span> 
	<span class="token operator">or</span> rt<span class="token punctuation">(</span>degrees<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>left<span class="token punctuation">(</span>degrees<span class="token punctuation">)</span> 
	<span class="token operator">or</span> lt<span class="token punctuation">(</span>degrees<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>circle<span class="token punctuation">(</span>radius<span class="token punctuation">,</span> extent<span class="token operator">=</span><span class="token boolean">None</span><span class="token punctuation">,</span> steps<span class="token operator">=</span><span class="token boolean">None</span><span class="token punctuation">)</span>

my_turtle<span class="token punctuation">.</span>speed<span class="token punctuation">(</span><span class="token number">0</span><span class="token punctuation">.</span><span class="token punctuation">.</span><span class="token number">10</span><span class="token punctuation">)</span>	<span class="token comment">#0 is fastest (no animation), then speed drops from 10 to 1</span>
my_turtle<span class="token punctuation">.</span>shape<span class="token punctuation">(</span><span class="token string">"arrow"</span> <span class="token operator">or</span> <span class="token string">"turtle"</span> <span class="token operator">or</span> <span class="token string">"circle"</span> <span class="token operator">or</span> <span class="token string">"square"</span> <span class="token operator">or</span> <span class="token string">"triangle"</span> <span class="token operator">or</span> <span class="token string">"classic"</span> <span class="token operator">or</span> <span class="token string">"blank"</span><span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>shapesize<span class="token punctuation">(</span>stretch_wid<span class="token operator">=</span><span class="token boolean">None</span><span class="token punctuation">,</span> stretch_len<span class="token operator">=</span><span class="token boolean">None</span><span class="token punctuation">,</span> outline<span class="token operator">=</span><span class="token boolean">None</span><span class="token punctuation">)</span> 
	<span class="token operator">or</span> my_turtle<span class="token punctuation">.</span>turtlesize<span class="token punctuation">(</span><span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>pensize<span class="token punctuation">(</span>lines<span class="token punctuation">)</span> 
	<span class="token operator">or</span> width<span class="token punctuation">(</span>lines<span class="token punctuation">)</span>

my_turtle<span class="token punctuation">.</span>color<span class="token punctuation">(</span>color<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>pencolor<span class="token punctuation">(</span>color<span class="token punctuation">)</span>
my_turtle<span class="token punctuation">.</span>fillcolor<span class="token punctuation">(</span>color<span class="token punctuation">)</span>

<span class="token comment">#turn off tracer</span>
my_turtle<span class="token punctuation">.</span>tracer<span class="token punctuation">(</span><span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">)</span>
<span class="token comment">#because tracer is off</span>
my_turtle<span class="token punctuation">.</span>update<span class="token punctuation">(</span><span class="token punctuation">)</span>

<span class="token comment">#only exit onclick</span>
window<span class="token punctuation">.</span>exitonclick<span class="token punctuation">(</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="file-manipulation---built-in-functions">File Manipulation - Built-in Functions</h2>
<pre class=" language-python"><code class="prism  language-python">myFile <span class="token operator">=</span> <span class="token builtin">open</span><span class="token punctuation">(</span><span class="token string">"path"</span><span class="token punctuation">)</span>	<span class="token comment">#open() returns a file object</span>
content <span class="token operator">=</span> myFile<span class="token punctuation">.</span>read<span class="token punctuation">(</span><span class="token punctuation">)</span>
myFile<span class="token punctuation">.</span>close<span class="token punctuation">(</span><span class="token punctuation">)</span>

<span class="token keyword">import</span> urllib
connection <span class="token operator">=</span> urllib<span class="token punctuation">.</span>urlopen<span class="token punctuation">(</span><span class="token string">"http://www.wdyl.com/profanity?q="</span><span class="token operator">+</span>text<span class="token punctuation">)</span>
output <span class="token operator">=</span> connection<span class="token punctuation">.</span>read<span class="token punctuation">(</span><span class="token punctuation">)</span>
<span class="token keyword">print</span><span class="token punctuation">(</span>output<span class="token punctuation">)</span>
connection<span class="token punctuation">.</span>close<span class="token punctuation">(</span><span class="token punctuation">)</span>
</code></pre>
<h2 id="class-definition">Class Definition</h2>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">class</span> <span class="token class-name">Parent</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token triple-quoted-string string">"""This String will be accessable using the __doc__ variable"""</span>
   money <span class="token operator">=</span> <span class="token string">"under zero"</span>
   state <span class="token operator">=</span> <span class="token string">"exausted"</span>
   
   <span class="token keyword">def</span> <span class="token function">__init__</span><span class="token punctuation">(</span>self<span class="token punctuation">,</span> last_name<span class="token punctuation">,</span> eye_color<span class="token punctuation">)</span><span class="token punctuation">:</span>
      self<span class="token punctuation">.</span>last_name <span class="token operator">=</span> last_name
      self<span class="token punctuation">.</span>eye_color <span class="token operator">=</span> eye_color

   <span class="token keyword">def</span> <span class="token function">show_info</span><span class="token punctuation">(</span>self<span class="token punctuation">)</span><span class="token punctuation">:</span>
      <span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Last Name - "</span> <span class="token operator">+</span> self<span class="token punctuation">.</span>last_name<span class="token punctuation">)</span>
      <span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Eye Color - "</span> <span class="token operator">+</span> self<span class="token punctuation">.</span>eye_color<span class="token punctuation">)</span>


<span class="token keyword">class</span> <span class="token class-name">Child</span><span class="token punctuation">(</span>Parent<span class="token punctuation">)</span><span class="token punctuation">:</span>
   state <span class="token operator">=</span> <span class="token string">"lively"</span>
   
   <span class="token keyword">def</span> <span class="token function">__init__</span><span class="token punctuation">(</span>self<span class="token punctuation">,</span> last_name<span class="token punctuation">,</span> eye_color<span class="token punctuation">,</span> number_of_toys<span class="token punctuation">)</span><span class="token punctuation">:</span>
      Parent<span class="token punctuation">.</span>__init__<span class="token punctuation">(</span>self<span class="token punctuation">,</span> last_name<span class="token punctuation">,</span> eye_color<span class="token punctuation">)</span>
      self<span class="token punctuation">.</span>number_of_toys <span class="token operator">=</span> number_of_toys

   <span class="token keyword">def</span> <span class="token function">show_info</span><span class="token punctuation">(</span>self<span class="token punctuation">)</span><span class="token punctuation">:</span>
      Parent<span class="token punctuation">.</span>show_info<span class="token punctuation">(</span>self<span class="token punctuation">)</span>
      <span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Number of Toys - "</span> <span class="token operator">+</span> <span class="token builtin">str</span><span class="token punctuation">(</span>self<span class="token punctuation">.</span>number_of_toys<span class="token punctuation">)</span><span class="token punctuation">)</span>
      <span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"State - "</span> <span class="token operator">+</span> self<span class="token punctuation">.</span>state<span class="token punctuation">)</span>

gabgoob <span class="token operator">=</span> Child<span class="token punctuation">(</span><span class="token string">"Ben Shanioob"</span><span class="token punctuation">,</span> <span class="token string">"Honey"</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">)</span>
<span class="token keyword">print</span> gabgoob<span class="token punctuation">.</span>money
gabgoob<span class="token punctuation">.</span>show_info<span class="token punctuation">(</span><span class="token punctuation">)</span>

Parent<span class="token punctuation">.</span>__doc__		<span class="token comment">#The class documentation string.</span>
Parent<span class="token punctuation">.</span>__module__	<span class="token comment">#The name of the module in which this class was defined.</span>
Parent<span class="token punctuation">.</span>__name__		<span class="token comment">#The name of the class.</span>
Child<span class="token punctuation">.</span>__bases__	<span class="token comment">#The classes from which this class inherits.</span>
</code></pre>

