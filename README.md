Download Link: https://assignmentchef.com/product/solved-50-004-homework-set2
<br>
<strong>Note: </strong>In this homework set, log denotes the natural logarithm, i.e. the logarithm in base <em>e</em>. Following the notation used in the textbook, we write <em>A</em>[1<em>..n</em>] to mean an array <em>A </em>indexed from 1 to <em>n</em>. This means the first entry of <em>A </em>is <em>A</em>[1].

<strong>Question 1. </strong>Give asymptotic upper and lower bounds for <em>T</em>(<em>n</em>) in each of the following recurrences. Assume that <em>T</em>(<em>n</em>) is constant for <em>n </em>≤ 2. Make your bounds as tight as possible, and justify your answers.     [5 points]

<strong>Question 2.</strong>

<ul>

 <li>Explain how insertion sort can be expressed as a recursive procedure, write a recurrence for the running time of this recursive procedure, and solve the recurrence to get an asymptotic upper bound for the running time. [3 points]</li>

 <li>For input size <em>n &gt; </em>3, will insertion sort <strong>always </strong>run slower than merge sort? Please justify your answer with a detailed example. [2 points]</li>

</ul>

<strong>Question 3. </strong>An inversion in an array <em>A</em>[1<em>..n</em>] is a pair (<em>i,j</em>) of indices such that <em>i &lt; j</em>, but <em>A</em>[<em>i</em>] <em>&gt; A</em>[<em>j</em>]. Given an array whose entries are all distinct integers, design an algorithm that returns as its output the number of inversions in the given array. Your algorithm must run in <em>O</em>(<em>n</em>log<em>n</em>) time. Please give your algorithm in pseudocode, and explain why your algorithm runs in <em>O</em>(<em>n</em>log<em>n</em>) time. (Hint: Modify merge sort.)

<strong>Question 4. </strong>Inspired by the idea of cutting a deck of cards, John has designed an algorithm that takes as input an integer array <em>A </em>sorted in ascending order, and gives as output a “cut” of <em>A </em>performed at a random index. The pseudocode is given below:

<strong>function </strong>John Cut(<em>A</em>)

<strong>Require: </strong><em>A</em>[1<em>..n</em>] is a sorted array with <strong>distinct </strong>integers.

1: <em>k </em>← random integer selected from [1<em>,…,n</em>]

2: <em>B </em>←array obtained after merging subarrays <em>A</em>[<em>k </em>+ 1<em>..n</em>] and <em>A</em>[1<em>..k</em>] in this given order 3: <strong>return </strong><em>B</em>.

Example: If <em>A </em>= [0<em>,</em>1<em>,</em>2<em>,</em>4<em>,</em>5<em>,</em>7], then one possible output for John Cut(<em>A</em>) is [4<em>,</em>5<em>,</em>7<em>,</em>0<em>,</em>1<em>,</em>2].

Design an algorithm that takes as its inputs an integer <em>t </em>and an integer array <em>B</em>, assumed to be the output <em>B </em>= John Cut(<em>A</em>) for some sorted array <em>A </em>with <strong>distinct </strong>integers, and that returns as its output the character string “yes” or “no”, representing whether <em>t </em>is an entry of <em>B</em>. Your algorithm must run in <em>O</em>(log<em>n</em>) time. Please give your algorithm in pseudocode, and explain why your algorithm runs in <em>O</em>(log<em>n</em>) time. [5 points]

1

<strong>Remark: </strong>The symbol ← is used frequently in pseudocode, and it means “gets” or “is assigned”. For example, when incrementing a variable e.g. what we think of as “<em>i </em>= <em>i </em>+ 1”, it would be clearer to write “<em>i </em>← <em>i </em>+ 1” instead. (For those who write in <em>L</em><sup>A</sup><em>T</em>E<em>X</em>, the command for this symbol is gets.)

<strong>Question 5. </strong>There are 25 horses among which you need to identify the fastest 3 horses. You can conduct a race among at most 5 horses to find out their relative speeds. At no point in the race are you able to determine the actual (absolute) speed of any horse. Determine the least number of races required to identify the top 3 fastest horses, and explain how you schedule the races.