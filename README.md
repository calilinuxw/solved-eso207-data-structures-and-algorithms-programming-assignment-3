Download Link: https://assignmentchef.com/product/solved-eso207-data-structures-and-algorithms-programming-assignment-3
<br>



<strong>Question 1                                     BST to Greater Tree</strong>

Given a binary search tree <em>T</em>, the <em>greater tree T</em><sup>0 </sup>corresponding to <em>T </em>is defined as follows:

<ul>

 <li>the tree structure of <em>T</em><sup>0 </sup>is the same as the tree structure of <em>T</em>.</li>

 <li>the value of a node <em>v </em>in <em>T</em><sup>0 </sup>is the sum of all the keys greater than or equal to the value of the key in the node <em>v </em>in <em>T</em>.</li>

</ul>

For example consider a BST <em>T </em>and its corresponding greater tree <em>T</em><sup>0</sup>.

(a) binary search tree <em>T                                         </em>(b) corresponding greater tree <em>T</em><sup>0</sup>

Given the preorder traversal of a BST <em>T</em>, you need to output the preorder traversal of the corresponding greater tree <em>T</em><sup>0</sup>.

<strong>Input:</strong>

First line will contain a single number <em>N</em>, denoting the number of nodes in the BST.

Next line will contain <em>N </em>integers, denoting the <strong>preorder traversal </strong>of the BST (all <em>N </em>numbers will be unique).

<strong>Output:</strong>

Output the preorder traversal of the corresponding greater tree.

<strong>Constraints:</strong>

<ul>

 <li>≤ <em>N </em>≤ 10<sup>5</sup></li>

</ul>

0 ≤ key value at a node ≤ 10<sup>5</sup>

<strong>Example:</strong>

<strong>Sample Input:</strong>

9

4          1 0 2 3 6 5 7 8

<strong>Sample Output:</strong>

30         36 36 35 33 21 26 15 8

<strong>Question 2                                  Covid spread</strong>

Moni is the head nurse at city hospital which has wards arranged in a rectangular grid shape with <em>R </em>rows and <em>C </em>columns.

You are given a <em>R</em>×<em>C </em>matrix <em>Mat </em>where each cell <em>Mat </em>can have values <strong>0</strong>, <strong>1 </strong>or <strong>2 </strong>which has the following meaning:

<ul>

 <li>: Empty ward</li>

 <li>: Wards without infected patients</li>

 <li>: Wards with infected patients</li>

</ul>

An infected patient at ward (<em>i,j</em>) can infect other uninfected patients at wards (<em>i </em>− 1<em>,j</em>), (<em>i </em>+ 1<em>,j</em>), (<em>i,j </em>− 1) and (<em>i,j </em>+ 1) (i.e. up, down, left and right) in one unit of time. Help Moni determine the minimum units of time after which there won’t remain any uninfected patient i.e all patients would be infected. If all patients are not infected after infinite units of time then simply return −1.

<strong>Input:</strong>

First line contains two integers <em>R </em>and <em>C</em>, the number of rows and columns. Next <em>R </em>lines contain the 2-D Matrix <strong>Mat </strong>with <em>C </em>entries per line.

<strong>Output:</strong>

Print the minimum units of time in which all patients will be infected or −1 if it is impossible.

<strong>Constraints:</strong>

<ul>

 <li>≤ <em>R,C </em>≤ 1000 0 ≤ <em>Mat</em>(<em>i,j</em>) ≤ 2</li>

</ul>

<strong>Example:</strong>

<strong>Sample Input:</strong>

3    5

<ul>

 <li>1 0               2               1</li>

</ul>

1    0    1    2    1

1    0    0    2    1

<strong>Sample Output: </strong>2

<strong>Explanation:</strong>

Patients at positions {0,0}, {0, 3}, {1, 3} and {2, 3} will infect patient at {0, 1},{1, 0},{0, 4}, {1, 2}, {1, 4}, {2, 4} during 1st unit time.

And, during 2nd unit time, patient at {1, 0} will get infected and will infect patient at {2, 0}. Hence, total <strong>2 </strong>unit of time is required to infect all patients.

<strong>Question 3                                   Number of Islands</strong>

In a <em>m</em>×<em>n </em>2D binary grid <em>A</em>, a cell with 1 represents land and a cell with 0 represents water. An <em>island </em>is a connected subset of 1’s surrounded by all 0’s. Two 1’s are said to be connected if they are horizontally or vertically adjacent.

Given such a grid find the total number of islands.

<strong>Input:</strong>

First line contains two integers <em>m </em>and <em>n</em>, the number of rows and columns. Next <em>m </em>lines contain the 2-D Matrix <em>A </em>with <em>n </em>entries per line.

<strong>Output:</strong>

Print single integer representing total number of islands present in the 2D grid <em>A</em>.

<strong>Constraints:</strong>

1 ≤ <em>m,n </em>≤ 300 0 ≤ grid value ≤ 1 <strong>Example:</strong>

<strong>Sample Input:</strong>

4    5

1    1    0    0    0

1    1    0    0    0

0    0    1    0    0

<ul>

 <li>0 0               1               1</li>

</ul>

<strong>Sample Output: </strong>3

<strong>Explanation:</strong>

(a) Different blocks represent islands

<strong>Question 4                                    Brother from different roots</strong>

You are given the preorder traversal of two BSTs <em>T</em><sub>1 </sub>and <em>T</em><sub>2 </sub>containing <em>n</em><sub>1 </sub>and <em>n</em><sub>2 </sub>nodes respectively, and a number <em>k</em>. Assume all values of <em>T</em><sub>1 </sub>and <em>T</em><sub>2 </sub>are distinct within that tree. The problem is to count the number of pairs of nodes such that the first node is from <em>T</em><sub>1 </sub>an the second node is from <em>T</em><sub>2</sub>, and the value of the sum of these two nodes equals <em>k</em>.

<strong>Input:</strong>

<ul>

 <li>First line will contain a single number <em>n</em><sub>1</sub>, denoting the number of nodes in the <em>T</em><sub>1</sub>.</li>

 <li>Second line will contain <em>n</em><sub>1 </sub>integers, denoting the preorder traversal of <em>T</em><sub>1 </sub>(all <em>n</em><sub>1 </sub>numbers are unique).</li>

 <li>Third line will contain a single number <em>n</em><sub>2</sub>, denoting the number of nodes in the <em>T</em><sub>2</sub>.</li>

 <li>Fourth line will contain <em>n</em><sub>2 </sub>integers, denoting the preorder traversal of <em>T</em><sub>2 </sub>(all <em>n</em><sub>2 </sub>numbers are unique).</li>

 <li>Next line will contain a single integer <em>k</em>.</li>

</ul>

<strong>Output:</strong>

Output the number of pairs from two BSTs whose sum is equal to a given value <em>k</em>.

<strong>Constraints:</strong>

<ul>

 <li>≤ <em>n</em><sub>1</sub><em>,n</em><sub>2 </sub>≤ 5000</li>

</ul>

−10<sup>9 </sup>≤ Node.Value ≤ 10<sup>9 </sup>−10<sup>9 </sup>≤ <em>k </em>≤ 10<sup>9</sup>

<strong>Example:</strong>

<strong>Sample Input:</strong>

3

<ul>

 <li>1 4</li>

</ul>

3

1     0 3

5


