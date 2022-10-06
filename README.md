Short List
==========
- [**Coding Challenge 1 - Java Coder**](#coding-challenge-1---java-coder)
- [**Coding Challenge 2 - Python & Java Coder**](#coding-challenge-2---python--java-coder)
- [**4 Swapping Techniques**](#4-swapping-techniques)
___________

## Coding Challenge 1 - Java Coder
**Java Code -**
```java
public class CodeXam{
    public static void main(String [] arr){
     Integer num1 = 100, num2 = 100, num3 = 500, num4 = 500;
        if(num3 == num4 ) {
            System.out.println("3");
        }else if(num1 == num2) {
            System.out.println("4");
        }else{
            System.out.println("2");
        }
    }
}
```
**Output -**
```
4
```
**Explanation -**
The output is 4 because the value of num1 and num2 are equal to 100 and the value of num3 and num4 are equal to 500. So, the output is 4 even num3 and num4 are equal to 500 but if we store it in int then the output will be 3.

## Coding Challenge 2 - Python & Java Coder
**Java Code -**
```java
public class CodeXam{
    public static void main(String[]args){
        int CodeXam = 0x000F;
        int Xam = 0x57;
        System.out.println(CodeXam & Xam);
    }
}
```
**Output -**
```
7
```
**Python Code -** 
```python
CodeXam = 0x000F
Xam = 0x57
print(CodeXam & Xam)

```
**Output -**
```
7
```
**Explanation -**
0x000F - 15
0x57 - 87 
15 in binary is 0000 1111
87 in binary is 0101 0111
**We know, and operator will return 1 if both the bits are 1 else it will return 0.
So, 0000 1111 & 0101 0111 = 0000 0111 = 7 in decimal.**

## 4 Swapping Techniques

<section class="main"><h2 id="example-1:-swap-two-numbers-in-java-using-temporary-variable" level="2">Example 1: Swap Two Numbers in Java Using Temporary Variable</h2><p>Let us think of a real-life example. Suppose you have a box containing a red ball and a box containing a black ball. You want to swap the balls in the two boxes.</p><p><strong>How will you do this?</strong></p><p>You can take the help of a temporary box. You can keep the black ball in the temporary box and keep the red ball in the box which contained the black ball. Later you can take the black ball from the temporary box and keep it in the box which contained the red ball initially.</p><p>

![Screenshot 2022-10-06 135545](https://user-images.githubusercontent.com/97989643/194261508-6a1bc0ac-95e6-470a-810e-acb84e875b2b.png)

</p><p><strong>How can we map this solution to a function?</strong></p><p>We will create a temporary variable and assign the value of the first variable to the temporary variable. Similar to how we took a temporary box in the box and ball example. later we will assign the value of the second variable to the first variable and then we assign the value of the temporary variable to the second variable, Just like how we changed the position of the balls in the box.</p><p><strong>Let us look at the code:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span style="color:#F92672">public</span><span> </span><span class="hljs-class" style="color:#F92672">class</span><span class="hljs-class"> </span><span class="hljs-class" style="color:#61aeee">Swap</span><span class="hljs-class"> </span><span>{
</span>
<span>    </span><span style="color:#F92672">public</span><span style="color:#61aeee"> </span><span style="color:#F92672">static</span><span style="color:#61aeee"> </span><span style="color:#F92672">void</span><span style="color:#61aeee"> </span><span style="color:#61aeee">main</span><span style="color:#61aeee">(String[] args)</span><span style="color:#61aeee"> </span><span>{
</span>
<span>        </span><span style="color:#F92672">int</span><span> a = </span><span style="color:#d19a66">10</span><span>, b = </span><span style="color:#d19a66">20</span><span>;
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;Before swapping the numbers:&quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>        
<span>        </span><span style="color:#F92672">int</span><span> temp = a;  </span><span style="color:#b18eb1;font-style:italic">//Temporary value is assigned with the value of the First variable</span><span>
</span><span>        a = b;         </span><span style="color:#b18eb1;font-style:italic">//The First variable is assigned with the value of the Second variable </span><span>
</span><span>        b = temp;      </span><span style="color:#b18eb1;font-style:italic">// The Second variable is assigned with the value of the Temporary variable i.e, the First variable</span><span>
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;After swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>    }
<!-- -->}
</code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Output:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span>Before swapping the numbers:
</span><span>First number = </span><span style="color:#d19a66">10</span><span>
</span><span>Second number = </span><span style="color:#d19a66">20</span><span>
</span>After swapping the numbers: 
<span>First number = </span><span style="color:#d19a66">20</span><span>
</span><span>Second number = </span><span style="color:#d19a66">10</span><span>
</span></code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p>As we can see in the output, the value of the first number and the second number is swapped using a <strong>temporary variable</strong>.</p></section>
<section class="main"><h2 id="example-2:-swap-two-numbers-in-java-without-using-a-temporary-variable" level="2">Example 2: Swap Two Numbers in Java Without Using a Temporary Variable</h2><p>Previously, we saw the swapping of two Numbers in java using a temporary variable. Now let us see how swapping two numbers in java without using a temporary variable.</p><ul>
<li><strong>Using Arithmetic Addition and Subtraction</strong>
We saw how to swap two numbers using a temporary variable. We can swap two numbers without using a temporary variable as well, i.e., by <strong>simple mathematics</strong>. Let us look at the code, and later we will understand the logic behind the code.</li>
</ul><p><strong>Code:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span style="color:#F92672">public</span><span> </span><span class="hljs-class" style="color:#F92672">class</span><span class="hljs-class"> </span><span class="hljs-class" style="color:#61aeee">Swap</span><span class="hljs-class"> </span><span>{
</span>
<span>    </span><span style="color:#F92672">public</span><span style="color:#61aeee"> </span><span style="color:#F92672">static</span><span style="color:#61aeee"> </span><span style="color:#F92672">void</span><span style="color:#61aeee"> </span><span style="color:#61aeee">main</span><span style="color:#61aeee">(String[] args)</span><span style="color:#61aeee"> </span><span>{
</span>
<span>        </span><span style="color:#F92672">int</span><span> a = </span><span style="color:#d19a66">10</span><span>, b = </span><span style="color:#d19a66">20</span><span>;
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;Before swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>
<!-- -->        a = a + b;
<!-- -->        b = a - b;
<!-- -->        a = a - b;
<!-- -->
<span>        System.out.println(</span><span style="color:#98c379">&quot;After swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>    }
<!-- -->}
</code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Output:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span>Before swapping the numbers:
</span><span>First number = </span><span style="color:#d19a66">10</span><span>
</span><span>Second number = </span><span style="color:#d19a66">20</span><span>
</span>After swapping the numbers: 
<span>First number = </span><span style="color:#d19a66">20</span><span>
</span><span>Second number = </span><span style="color:#d19a66">10</span><span>
</span></code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Explanation</strong>
Now that we have seen the code and the output, let us understand what happened in the code that led to the swapping of two numbers. The <strong>swapping of numbers</strong> occurred in the <span class="highlight--red">11, 12</span>, and <span class="highlight--red">13th lines</span>.</p><ul>
<li>In the line 11, <span class="highlight--red">a = a + b</span>, <span class="highlight--red">a</span> is assigned the value of <span class="highlight--red">a + b</span>, i.e., the sum of given numbers. In this case, <span class="highlight--red">a = 10 + 20</span>, i.e., <span class="highlight--red">a = 30</span>.</li>
<li>In the next step, i.e., <span class="highlight--red">b = a - b</span>, we take the difference between the sum (of a and b) and <span class="highlight--red">b</span>. Since <span class="highlight--red">b</span> is subtracted from the sum of <span class="highlight--red">a</span> and <span class="highlight--red">b</span>, we got the value of <span class="highlight--red">a</span>. Hence, using <span class="highlight--red">b = a - b</span>, the original value of <span class="highlight--red">a</span> is assigned to <span class="highlight--red">b</span>. In this case, we get <span class="highlight--red">b = 30 - 20</span>, i.e., <span class="highlight--red">b = 10</span>.</li>
<li>Till now, we have assigned the value of <span class="highlight--red">a</span> in <span class="highlight--red">b</span> but we are yet to assign the value of <span class="highlight--red">b</span> in <span class="highlight--red">a</span>. This is also simple to do. If we subtract the original value of <span class="highlight--red">a</span> from the <span class="highlight--red">sum</span>, then we will end up with the value of <span class="highlight--red">b</span>. So, with <span class="highlight--red">a = a - b</span>, the original value of <span class="highlight--red">a</span> (currently stored in <span class="highlight--red">b</span>) is subtracted from the sum (currently stored in <span class="highlight--red">a</span>). Hence, now <span class="highlight--red">a</span> contains the original value of <span class="highlight--red">b</span>. So, in the last step, i.e., <span class="highlight--red">a = a - b</span>, we get <span class="highlight--red">a = 30 - 10</span>, i.e., <span class="highlight--red">a = 20</span></li>
</ul><p><strong>As you can see, we just swapped the two numbers without using a temporary variable</strong>.</p></section>
<section class="tip"><p><strong>Note:</strong>
If the value of <span class="highlight--red">a</span> and <span class="highlight--red">b</span> are too large, this approach may fail due to arithmetic overflow as addition may go out of the integer range.</p></section>
<section><ul>
<li><strong>Using Arithmetic Multiplication and Division</strong></li>
</ul><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span style="color:#F92672">public</span><span> </span><span class="hljs-class" style="color:#F92672">class</span><span class="hljs-class"> </span><span class="hljs-class" style="color:#61aeee">Swap</span><span class="hljs-class"> </span><span>{
</span>
<span>    </span><span style="color:#F92672">public</span><span style="color:#61aeee"> </span><span style="color:#F92672">static</span><span style="color:#61aeee"> </span><span style="color:#F92672">void</span><span style="color:#61aeee"> </span><span style="color:#61aeee">main</span><span style="color:#61aeee">(String[] args)</span><span style="color:#61aeee"> </span><span>{
</span>
<span>        </span><span style="color:#F92672">int</span><span> a = </span><span style="color:#d19a66">10</span><span>, b = </span><span style="color:#d19a66">20</span><span>;
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;Before swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>
<!-- -->        a = a * b;
<!-- -->        b = a / b;
<!-- -->        a = a / b;
<!-- -->
<span>        System.out.println(</span><span style="color:#98c379">&quot;After swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>    }
<!-- -->}
</code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Output:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span>Before swapping the numbers:
</span><span>First number = </span><span style="color:#d19a66">10</span><span>
</span><span>Second number = </span><span style="color:#d19a66">20</span><span>
</span>After swapping the numbers: 
<span>First number = </span><span style="color:#d19a66">20</span><span>
</span><span>Second number = </span><span style="color:#d19a66">10</span><span>
</span></code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Explanation</strong>
Like the previous method, even though this method is implemented, we use <strong>multiplication and division to swap</strong> two numbers that we can easily understand from the above code.</p></section>
<section class="tip"><p><strong>Note:</strong>
The arithmetic multiplication and division method to swap two numbers work fine with <strong>non-zero numbers</strong>. But this approach won&#x27;t work if any one of the numbers is <strong><span class="highlight--red">0</span> because the product becomes <span class="highlight--red">0</span></strong> (in line <span class="highlight--red">11</span>) irrespective of the other number.</p></section>
<section><ul>
<li><strong>Using Bitwise XOR operator</strong></li>
</ul><p>The XOR of two numbers <span class="highlight--red">a</span> and <span class="highlight--red">b</span> returns a number that has all the bits as <span class="highlight--red">1</span> wherever bits of <span class="highlight--red">a</span> and <span class="highlight--red">b</span> differ.</p><p><strong>Example</strong>: <span class="highlight--red">5</span> is represented as <span class="highlight--red">101</span> in binary, <span class="highlight--red">4</span> as <span class="highlight--red">100</span> in binary. The XOR of <span class="highlight--red">5</span> and <span class="highlight--red">4</span> is <span class="highlight--red">001</span>, i.e., <span class="highlight--red">1</span>.</p>
<div style="overflow:auto"><table><thead><tr><th style="text-align:center"></th><th style="text-align:center">Decimal</th><th style="text-align:center">Binary</th></tr></thead><tbody><tr><td style="text-align:center">Number</td><td style="text-align:center">5</td><td style="text-align:center">101</td></tr><tr><td style="text-align:center">Number</td><td style="text-align:center">4</td><td style="text-align:center">100</td></tr><tr><td style="text-align:center">Bitwise XOR</td><td style="text-align:center">1</td><td style="text-align:center">001</td></tr></tbody></table></div><p><strong>Let us see how can we use it to swap two numbers</strong>.</p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span style="color:#F92672">public</span><span> </span><span class="hljs-class" style="color:#F92672">class</span><span class="hljs-class"> </span><span class="hljs-class" style="color:#61aeee">Swap</span><span class="hljs-class"> </span><span>{
</span>
<span>    </span><span style="color:#F92672">public</span><span style="color:#61aeee"> </span><span style="color:#F92672">static</span><span style="color:#61aeee"> </span><span style="color:#F92672">void</span><span style="color:#61aeee"> </span><span style="color:#61aeee">main</span><span style="color:#61aeee">(String[] args)</span><span style="color:#61aeee"> </span><span>{
</span>
<span>        </span><span style="color:#F92672">int</span><span> a = </span><span style="color:#d19a66">10</span><span>, b = </span><span style="color:#d19a66">5</span><span>;
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;Before swapping the numbers:&quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>        
<span>        a = a ^ b; </span><span style="color:#b18eb1;font-style:italic">// The value of a becomes 15</span><span>
</span><span>        b = a ^ b; </span><span style="color:#b18eb1;font-style:italic">// The value of b becomes 10</span><span>
</span><span>        a = a ^ b; </span><span style="color:#b18eb1;font-style:italic">// The value of a becomes 5</span><span>
</span>
<span>        System.out.println(</span><span style="color:#98c379">&quot;After swapping the numbers: &quot;</span><span>);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;First number = &quot;</span><span> + a);
</span><span>        System.out.println(</span><span style="color:#98c379">&quot;Second number = &quot;</span><span> + b);
</span>    }
<!-- -->}
</code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Output:</strong></p><pre><div class="code-box-module_snippetContainer__Zspjo"><pre style="display:block;overflow-x:auto;padding:0.5em;color:#abb2bf;background:#282c34"><code class="language-java" style="white-space:pre"><span>Before swapping the numbers:
</span><span>First number = </span><span style="color:#d19a66">10</span><span>
</span><span>Second number = </span><span style="color:#d19a66">5</span><span>
</span>After swapping the numbers: 
<span>First number = </span><span style="color:#d19a66">5</span><span>
</span><span>Second number = </span><span style="color:#d19a66">10</span><span>
</span></code></pre><a class="tappable btn-icon code-box-module_copyIcon__JbgTP" data-for="copy" data-tip="Copied" data-place="left" data-effect="solid" data-event="CopyTooltipEvent" data-scroll-hide="true"><i class="icon-copy code-box-module_copy_icon__ftVgJ"></i></a></div></pre><p><strong>Explanation</strong></p><p><strong>In this method, we made use of bitwise XOR operator. Bitwise XOR has two interesting properties</strong>:</p><ul>
<li><span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><msup><mi>x</mi><mi>x</mi></msup><mo>=</mo><mn>0</mn></mrow><annotation encoding="application/x-tex">x ^ x = 0</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.664392em;"></span><span class="strut bottom" style="height:0.664392em;vertical-align:0em;"></span><span class="base"><span class="mord"><span class="mord mathit">x</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.664392em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">x</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord">0</span></span></span></span></span></li>
<li><span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><msup><mi>x</mi><mn>0</mn></msup><mo>=</mo><mi>x</mi></mrow><annotation encoding="application/x-tex">x ^ 0 = x</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.8141079999999999em;"></span><span class="strut bottom" style="height:0.8141079999999999em;vertical-align:0em;"></span><span class="base"><span class="mord"><span class="mord mathit">x</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.8141079999999999em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">0</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord mathit">x</span></span></span></span></span></li>
</ul><p>So, in line <span class="highlight--red">11</span>, <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><mi>a</mi><mo>=</mo><msup><mi>a</mi><mi>b</mi></msup></mrow><annotation encoding="application/x-tex">a = a ^ b</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.849108em;"></span><span class="strut bottom" style="height:0.849108em;vertical-align:0em;"></span><span class="base"><span class="mord mathit">a</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span></span></span></span></span>, the value of <span class="highlight--red">a</span> is changed to <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><msup><mi>a</mi><mi>b</mi></msup></mrow><annotation encoding="application/x-tex">a ^ b</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.849108em;"></span><span class="strut bottom" style="height:0.849108em;vertical-align:0em;"></span><span class="base"><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span></span></span></span></span>.
In line <span class="highlight--red">12</span>, <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><mi>b</mi><mo>=</mo><msup><mi>a</mi><mi>b</mi></msup></mrow><annotation encoding="application/x-tex">b = a ^ b</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.849108em;"></span><span class="strut bottom" style="height:0.849108em;vertical-align:0em;"></span><span class="base"><span class="mord mathit">b</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span></span></span></span></span>. So, <span class="highlight--red">b</span> becomes <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><msup><mi>a</mi><mi>b</mi></msup><mo>=</mo><mo>(</mo><msup><mi>a</mi><mi>b</mi></msup><msup><mo>)</mo><mi>b</mi></msup><mo>=</mo><msup><mi>a</mi><mrow><msup><mi>b</mi><mo>(</mo></msup><mi>b</mi><mo>)</mo></mrow></msup><mo>=</mo><msup><mi>a</mi><mn>0</mn></msup><mo>=</mo><mi>a</mi></mrow><annotation encoding="application/x-tex">a ^ b = (a ^ b) ^  b = a ^ {b ^ (b)} = a ^ 0 = a</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:1.0396999999999998em;"></span><span class="strut bottom" style="height:1.2896999999999998em;vertical-align:-0.25em;"></span><span class="base"><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mopen">(</span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mclose"><span class="mclose">)</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:1.0396999999999998em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight"><span class="mord mathit mtight">b</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.9667142857142857em;"><span style="top:-2.966714285714285em;margin-right:0.07142857142857144em;"><span class="pstrut" style="height:2.5357142857142856em;"></span><span class="sizing reset-size3 size1 mtight"><span class="mopen mtight">(</span></span></span></span></span></span></span></span><span class="mord mathit mtight">b</span><span class="mclose mtight">)</span></span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.8141079999999999em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">0</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord mathit">a</span></span></span></span></span>. Thus, the value of <span class="highlight--red">a</span> is now stored in <span class="highlight--red">b</span>.
And, in line <span class="highlight--red">13</span>, <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><mi>a</mi><mo>=</mo><msup><mi>a</mi><mi>b</mi></msup></mrow><annotation encoding="application/x-tex">a = a ^ b</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.849108em;"></span><span class="strut bottom" style="height:0.849108em;vertical-align:0em;"></span><span class="base"><span class="mord mathit">a</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span></span></span></span></span>. So, <span class="highlight--red">a</span> becomes <span><span class="katex"><span class="katex-mathml"><math><semantics><mrow><msup><mi>a</mi><mi>b</mi></msup><mo>=</mo><mo>(</mo><msup><mi>a</mi><mi>b</mi></msup><msup><mo>)</mo><mi>a</mi></msup><mo>=</mo><mo>(</mo><msup><mi>a</mi><mi>a</mi></msup><msup><mo>)</mo><mi>b</mi></msup><mo>=</mo><msup><mn>0</mn><mi>b</mi></msup><mo>=</mo><mi>b</mi></mrow><annotation encoding="application/x-tex">a ^ b = (a ^ b) ^ a = (a ^ a) ^ b = 0 ^ b = b</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="strut" style="height:0.849108em;"></span><span class="strut bottom" style="height:1.099108em;vertical-align:-0.25em;"></span><span class="base"><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mopen">(</span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mclose"><span class="mclose">)</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.664392em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">a</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mopen">(</span><span class="mord"><span class="mord mathit">a</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.664392em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">a</span></span></span></span></span></span></span></span><span class="mclose"><span class="mclose">)</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord"><span class="mord">0</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.849108em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathit mtight">b</span></span></span></span></span></span></span></span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mrel">=</span><span class="mord rule" style="margin-right:0.2777777777777778em;"></span><span class="mord mathit">b</span></span></span></span></span>. Thus, the value of <span class="highlight--red">b</span> is now stored in <span class="highlight--red">a</span> as well.</p><p>In this way, we successfully swapped the numbers <span class="highlight--red">a</span> and <span class="highlight--red">b</span> using the bitwise XOR operator.</p></section>
<section class="tip"><p><strong>Note:</strong>
The above method to swap two numbers works fine with non-zero numbers. But this approach won&#x27;t work if any one of the numbers is <span class="highlight--red">0</span> because the XOR will be equal to the non-zero number and the same will be assigned to both the numbers.</p></section>
<section class="summary"><h2 id="conclusion" level="2">Conclusion</h2><ul>
<li>Swapping of two numbers in Java can be done using a <strong>temporary variable</strong>.</li>
<li>Simple arithmetic operations such as <em>addition and subtraction</em> and <em>multiplication and division</em> can also be used in swapping two numbers in java.</li>
<li>Bitwise <strong>XOR operator</strong> can be used in the swapping of two numbers in Java.</li>
</ul></section></div><div class="__react_component_tooltip t8b0a9816-5df1-4bcf-acd3-1ef4d4689c5f place-top type-dark" id="copy" data-id="tooltip">


