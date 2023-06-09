Download Link: https://assignmentchef.com/product/solved-csce-121-lab-5
<br>
This lab differs from the previous ones as there are no new programming exercises. It is intended to give you an opportunity to go back over the previous weeks’ lab exercises and to complete those questions you were unable to finish previously. This may include questions where you have <em>an</em> answer, but for which you harbor suspicions that your solution only works in particular limited cases or might be improved in some way.

If you’ve found the questions to be easy so far, then use this lab to write radically new programs as answers to the most interesting of the questions. For example, if you used a loop in your previous answer, try to do it with a recursive function call instead.

So what exactly is this lab?

Your lab time is best spent getting help on the trickiest questions in the previous labs:

<ul>

 <li><a href="http://robotics.cs.tamu.edu/dshell/cs121/l1/l1.html">Lab One</a></li>

 <li><a href="http://robotics.cs.tamu.edu/dshell/cs121/l2/l2.html">Lab Two</a></li>

 <li><a href="http://robotics.cs.tamu.edu/dshell/cs121/l3/l3.html">Lab Three</a></li>

 <li><a href="http://robotics.cs.tamu.edu/dshell/cs121/l4/l4.html">Lab Four</a></li>

 <li>Quiz/Test Practice Material</li>

</ul>

Here are some questions that are intended as practice questions for the quizzes and midterm exams. Try to do them without using a computer or any external help, but then carefully check your answers using g++.

<h3>Question 1</h3>

#include &lt;iostream&gt;using namespace std; void func-x(int p[4]){    int i=10;    p=&amp;i;    cout &lt;&lt; p[0]} int main(){    int arr[4] = {1, 2, 3, 4}    func-x(arr);    cout &lt;&lt; arr[0];    return 0;}

What will be the output of the above program?

<ol>

 <li>10 10</li>

</ol>

<ol>

 <li>Compiler Error</li>

 <li>10 1</li>

 <li>Undefined Behavior</li>

 <li>1 10</li>

</ol>

<h3>Question 2</h3>

#include &lt;iostream&gt;using namespace std; int main(){    int arr[4] = {1, 2, 3, 4};    int p[4];    p=arr;    cout &lt;&lt; p[1];}

What will be the output?

<ol>

 <li>1</li>

</ol>

<ol>

 <li>Compile time error</li>

 <li>Undefined Behavior</li>

 <li>2</li>

 <li>{2, 3, 4}</li>

</ol>

<h3>Question 3</h3>

Which of the following is an illegal declaration?

<ol>

 <li>int a=0, b = 1, c=2; int array[3] = {a, b, c}</li>

</ol>

<ol>

 <li>int size = 3; int array[size];</li>

 <li>int size = 3; int array[size] = {1, 2, 3};</li>

 <li>int array[3] = {1, 2, 3, 4};</li>

 <li>All of the above</li>

</ol>

<h3>Question 4</h3>

#include &lt;iostream&gt;using namespace std; int main(){      int arr[5] = {1,2,3,4,5};      int i = -1;      cout &lt;&lt; arr[5];      return 0;}

What will be the output of the above program?

<ol>

 <li>Garbage/undefined value</li>

</ol>

<ol>

 <li>5</li>

 <li>6</li>

 <li>0</li>

 <li>None of the above</li>

</ol>

<h3>Question 5</h3>

#include &lt;iostream&gt;using namespace std; int main(){        int a[5] = {51, 1, 5, 20, 25};        int x, y, z;        x = ++a[1];        y = a[1]++;        z = a[x++];        cout &lt;&lt; x &lt;&lt; ” ” &lt;&lt; y &lt;&lt; ” ” &lt;&lt; z;        return 0;}

What will be the output of the above program?

<ol>

 <li>2, 3, 20</li>

</ol>

<ol>

 <li>2, 1, 5</li>

 <li>2, 2, 5</li>

 <li>1, 2, 5</li>

 <li>3, 2, 5</li>

</ol>

<h3>Question 6</h3>

An array’s elements are always stored in ________ memory locations.

<ol>

 <li>Sequential</li>

</ol>

<ol>

 <li>Random</li>

 <li>Sequential and Random</li>

 <li>Sometimes sequential and sometimes random</li>

 <li>None of the above</li>

</ol>

<h3>Question 7</h3>

#include &lt;iostream&gt;using namespace std; int main(){    char str[5] = “XYZ”;    cout &lt;&lt; str[3];    return 0;}

What will be the output of the above program?

<ol>

 <li>XYZ</li>

</ol>

<ol>

 <li>Nothing will be printed</li>

 <li>Z</li>

 <li>0</li>

 <li> </li>

</ol>

<h3>Question 8</h3>

#include &lt;iostream&gt;using namespace std; int main(){    int array[] = {10, 20, 40, 50};    cout &lt;&lt; 3[array];    return 0;}

What will be output?

<ol>

 <li>40</li>

</ol>

<ol>

 <li>Compilation Error</li>

 <li>30</li>

 <li>50</li>

 <li>150</li>

</ol>

<h3>Question 9</h3>

#include &lt;iostream&gt;using namespace std; int main(){    int i,j,k;    for (i=1; i&lt;=5; i++) {        for (j=5; j&gt;=i; j–) {            cout &lt;&lt; ” “;        }        for (k=1; k&lt;=i; k++) {            cout &lt;&lt; “*”;        }        cout &lt;&lt; endl;    }    return 0;}

What is output?

<ol>

 <li>* * *c.      * * *d.    * * * *</li>

 <li>* * * * *</li>

 <li>* * * h.  * * * i.  * * * *j.  * * * * *</li>

 <li></li>

 <li>* * *n.    * * *o.   * * * *p.  * * * * *</li>

 <li></li>

 <li>*        * *t.      * * *u.    * * * *v.  * * * * *w.    * * * *x.      * * *y.        * *z.          *</li>

 <li></li>

 <li>*                   * * *dd.                 * * * * *ee.               * * * * * * *ff.             * * * * * * * * *gg.           * * * * * * * * * * *</li>

 <li></li>

</ol>

<h3>Question 10</h3>

#include &lt;iostream&gt;using namespace std; void modify(int &amp;num1, int num2){    num1 += 2;    num2 += 1;} int main(){    int A = 20, B = 4;    modify(A, B);    cout &lt;&lt; A &lt;&lt; “, ” &lt;&lt; B &lt;&lt; endl;    modify(B, A);    cout &lt;&lt; A &lt;&lt; “, ” &lt;&lt; B &lt;&lt; endl;    return 0;}

What is output?

<ol>

 <li>22, 424, 5</li>

</ol>

<ol>

 <li>20, 420, 4</li>

 <li>22, 422, 6</li>

 <li>20, 420, 4</li>

 <li>22, 524, 6</li>

</ol>

<h3>Question 11</h3>

#include &lt;iostream&gt;using namespace std; void order(float my_list[], const int size){    float next_min, temp;    int location;        for(int i=0;i&lt;size;i++)    {        next_min = my_list[i];        location = i:                for(/* complete me */)        {            if(my_list[j] &lt; next_min)            {                next_min = my_list[j];                location = j;            }        }                //Swap the values        temp = my_list[i];        my_list[i] = my_list[location];        my_list[location] = temp;    }} int main(){    const int size = 5;    float my_list[size] = {2.3f, 0.0f, 1.2f, -9.3f, 8.4f};    order(my_list, size);        for(int i=0;i&lt;size;i++)    {        cout &lt;&lt; my_list[i] &lt;&lt; ” “;    }}

Fill in the incomplete for loop so that at the j<sup>th</sup> index, the value at j and the smallest value of the remaining list (j+1 to end) are swapped.

This method of sorting is known as the <em>selection sort</em>.

<h3>Question 12</h3>

#include &lt;iostream&gt;using namespace std; int main(){    int a[7] = {1, 2, 3, 4, 5, 6, 7};    int sum;    int i;    for (i=0; i&lt;7; i++)    {        sum += a[i];    }    cout &lt;&lt; sum &lt;&lt; endl;    return 0;}

What is the output?

<ol>

 <li>28</li>

</ol>

<ol>

 <li>21</li>

 <li>Segmentation Fault</li>

 <li>Compiler Error</li>

 <li>None of the above</li>

</ol>

<h3>Question 13</h3>

#include &lt;iostream&gt;using namespace std; int main(){    for (int i=0; i&lt;3; i++)    {        for (int i=0; i&lt;3; i++)        {            cout &lt;&lt; i &lt;&lt; ” “;        }    }    return 0;}

What is the output?

<ol>

 <li>Segmentation Fault</li>

</ol>

<ol>

 <li>Compiler Error</li>

 <li>0 1 2 0 1 2 0 1 2</li>

 <li>0 1 2 3 4 5 6 7 8</li>

 <li>0 1 2 3 4 5 6 7 8 9</li>

</ol>

<h3>Question 14</h3>

#include &lt;iostream&gt;using namespace std; int main(){    for (int i=0; i&lt;3; i++)    {        int number = i;        while (number &lt; 3)        {            number++;        }    }    cout &lt;&lt; number &lt;&lt; endl;    return 0;}

What is the output?

<ol>

 <li>9</li>

</ol>

<ol>

 <li>3</li>

 <li>6</li>

 <li>Segmentation Fault</li>

 <li>Compiler Error</li>

</ol>

<h3>Question 15</h3>

#include &lt;iostream&gt;using namespace std; int main(){    float f = 0.7;    if (f == 0.7)        cout &lt;&lt; “Yes” &lt;&lt; endl;    else        cout &lt;&lt; “No” &lt;&lt; endl;    return 0;}

What’s the output?

<ol>

 <li>Yes</li>

</ol>

<ol>

 <li>No</li>

 <li>Nothing (No output given)</li>

 <li>Segmentation Fault</li>

 <li>Compiler Error</li>

</ol>