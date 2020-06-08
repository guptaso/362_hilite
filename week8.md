# A3: Code Review Hands On
## Code Block 1
```
# Example 1
def my_func(a,b):
    x = a
    for i in range(b):
        a *= x
    return a
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Example 1</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">my_func</span>(a,b):
    x <span style="color: #333333">=</span> a
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(b):
        a <span style="color: #333333">*=</span> x
    <span style="color: #008800; font-weight: bold">return</span> a
</pre></td></tr></table></div>

## Code Block 2
```
def to_the_n(val, n):
    """Returns the val raised to the n"""
    result = val
    for i in range(n-1):
        result *= val
    return result
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">to_the_n</span>(val, n):
    <span style="color: #DD4422">&quot;&quot;&quot;Returns the val raised to the n&quot;&quot;&quot;</span>
    result <span style="color: #333333">=</span> val
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(n<span style="color: #333333">-</span><span style="color: #0000DD; font-weight: bold">1</span>):
        result <span style="color: #333333">*=</span> val
    <span style="color: #008800; font-weight: bold">return</span> result
</pre></td></tr></table></div>

## Code Block 3
```
def random_int(num):
    """Returns a random int that is 0 < and < num"""
    # return random.randint(0, num) This includes 0 and num, which is wrong
    return random.randit(1,num-1)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">random_int</span>(num):
    <span style="color: #DD4422">&quot;&quot;&quot;Returns a random int that is 0 &lt; and &lt; num&quot;&quot;&quot;</span>
    <span style="color: #888888"># return random.randint(0, num) This includes 0 and num, which is wrong</span>
    <span style="color: #008800; font-weight: bold">return</span> random<span style="color: #333333">.</span>randit(<span style="color: #0000DD; font-weight: bold">1</span>,num<span style="color: #333333">-</span><span style="color: #0000DD; font-weight: bold">1</span>)
</pre></td></tr></table></div>

## Code Block 4
```
def random_int(max_int):
    """Returns a random int that is 0 < and < max_int"""
    return random.randit(1, max_int-1)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">random_int</span>(max_int):
    <span style="color: #DD4422">&quot;&quot;&quot;Returns a random int that is 0 &lt; and &lt; max_int&quot;&quot;&quot;</span>
    <span style="color: #008800; font-weight: bold">return</span> random<span style="color: #333333">.</span>randit(<span style="color: #0000DD; font-weight: bold">1</span>, max_int<span style="color: #333333">-</span><span style="color: #0000DD; font-weight: bold">1</span>)
</pre></td></tr></table></div>

## Code Block 5
```
def check_if_empty(str):
    """Returns True if the string is empty"""
    empty = False
    if len(str) == 0:
        empty = True
    return empty
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">check_if_empty</span>(<span style="color: #007020">str</span>):
    <span style="color: #DD4422">&quot;&quot;&quot;Returns True if the string is empty&quot;&quot;&quot;</span>
    empty <span style="color: #333333">=</span> <span style="color: #007020">False</span>
    <span style="color: #008800; font-weight: bold">if</span> <span style="color: #007020">len</span>(<span style="color: #007020">str</span>) <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
        empty <span style="color: #333333">=</span> <span style="color: #007020">True</span>
    <span style="color: #008800; font-weight: bold">return</span> empty
</pre></td></tr></table></div>

## Code Block 6
```
def check_if_empty(val):
    """Returns True if the string is empty"""
    return len(val) == 0
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">check_if_empty</span>(val):
    <span style="color: #DD4422">&quot;&quot;&quot;Returns True if the string is empty&quot;&quot;&quot;</span>
    <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">len</span>(val) <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>
</pre></td></tr></table></div>

## Code Block 7
```
# Pull request 1
def my_func(x):


    return x**2
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 1</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">my_func</span>(x):


    <span style="color: #008800; font-weight: bold">return</span> x<span style="color: #333333">**</span><span style="color: #0000DD; font-weight: bold">2</span>
</pre></td></tr></table></div>

## Code Block 8
```
# Pull request 2
def create_odds(num):
    """Creates a list of len(num) of random odd numbers between 1 and 1000"""
    num_list = []
    for i in range(0, num):
        new_num = 2
        while new_num % 2 == 0:
            new_num = random.randint(1, 1000)
        num_list.append(new_num)
    return num_list


def create_evens(num):
    """Creates a list of len(num) of random even numbers between 1 and 1000"""
    num_list = []
    for i in range(0, num):
        new_num = 1
        while new_num % 2 != 0:
            new_num = random.randint(1, 1000)
        num_list.append(new_num)
    return num_list
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%"> 1
 2
 3
 4
 5
 6
 7
 8
 9
10
11
12
13
14
15
16
17
18
19
20
21</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 2</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">create_odds</span>(num):
    <span style="color: #DD4422">&quot;&quot;&quot;Creates a list of len(num) of random odd numbers between 1 and 1000&quot;&quot;&quot;</span>
    num_list <span style="color: #333333">=</span> []
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>, num):
        new_num <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">2</span>
        <span style="color: #008800; font-weight: bold">while</span> new_num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
            new_num <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">1</span>, <span style="color: #0000DD; font-weight: bold">1000</span>)
        num_list<span style="color: #333333">.</span>append(new_num)
    <span style="color: #008800; font-weight: bold">return</span> num_list


<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">create_evens</span>(num):
    <span style="color: #DD4422">&quot;&quot;&quot;Creates a list of len(num) of random even numbers between 1 and 1000&quot;&quot;&quot;</span>
    num_list <span style="color: #333333">=</span> []
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>, num):
        new_num <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">1</span>
        <span style="color: #008800; font-weight: bold">while</span> new_num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">!=</span> <span style="color: #0000DD; font-weight: bold">0</span>:
            new_num <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">1</span>, <span style="color: #0000DD; font-weight: bold">1000</span>)
        num_list<span style="color: #333333">.</span>append(new_num)
    <span style="color: #008800; font-weight: bold">return</span> num_list
</pre></td></tr></table></div>

## Code Block 9
```
# Pull request 2
def create_odds(num):
    """Creates a list of len(num) of random odd numbers between 1 and 1000"""
    num_list = []
    for i in range(0, num):
        new_num = 2
        while new_num % 2 == 0:
            new_num = random.randint(1, 1000)
        num_list.append(new_num)
    return num_list


def create_evens(num):
    """Creates a list of len(num) of random even numbers between 1 and 1000"""
    num_list = []
    for i in range(0, num):
        new_num = 1
        while new_num % 2 != 0:
            new_num = random.randint(1, 1000)
        num_list.append(new_num)
    return num_list
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%"> 1
 2
 3
 4
 5
 6
 7
 8
 9
10
11
12
13
14
15
16
17
18
19
20
21</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 2</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">create_odds</span>(num):
    <span style="color: #DD4422">&quot;&quot;&quot;Creates a list of len(num) of random odd numbers between 1 and 1000&quot;&quot;&quot;</span>
    num_list <span style="color: #333333">=</span> []
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>, num):
        new_num <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">2</span>
        <span style="color: #008800; font-weight: bold">while</span> new_num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
            new_num <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">1</span>, <span style="color: #0000DD; font-weight: bold">1000</span>)
        num_list<span style="color: #333333">.</span>append(new_num)
    <span style="color: #008800; font-weight: bold">return</span> num_list


<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">create_evens</span>(num):
    <span style="color: #DD4422">&quot;&quot;&quot;Creates a list of len(num) of random even numbers between 1 and 1000&quot;&quot;&quot;</span>
    num_list <span style="color: #333333">=</span> []
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>, num):
        new_num <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">1</span>
        <span style="color: #008800; font-weight: bold">while</span> new_num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">!=</span> <span style="color: #0000DD; font-weight: bold">0</span>:
            new_num <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">1</span>, <span style="color: #0000DD; font-weight: bold">1000</span>)
        num_list<span style="color: #333333">.</span>append(new_num)
    <span style="color: #008800; font-weight: bold">return</span> num_list
</pre></td></tr></table></div>

## Code Block 10
```
# Pull request 3
def check_for_val(self, val):
    """This member function checks to see if val exists in the class member
    values and returns True if found"""
    for i in range(len(self.values)):
        if self.values[i] == val:
            return True
    return False
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7
8</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 3</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">check_for_val</span>(<span style="color: #007020">self</span>, val):
    <span style="color: #DD4422">&quot;&quot;&quot;This member function checks to see if val exists in the class member</span>
<span style="color: #DD4422">    values and returns True if found&quot;&quot;&quot;</span>
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #007020">len</span>(<span style="color: #007020">self</span><span style="color: #333333">.</span>values)):
        <span style="color: #008800; font-weight: bold">if</span> <span style="color: #007020">self</span><span style="color: #333333">.</span>values[i] <span style="color: #333333">==</span> val:
            <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">True</span>
    <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">False</span>
</pre></td></tr></table></div>

## Code Block 11
```
# Pull request 4
def get_val_index(arr, val):
    """Searches arr for val and returns the index if found, otherwise -1"""
    index = -1
    for i in range(len(arr)):
        if arr[i] == val:
            index = i
            break
    return index
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7
8
9</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 4</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">get_val_index</span>(arr, val):
    <span style="color: #DD4422">&quot;&quot;&quot;Searches arr for val and returns the index if found, otherwise -1&quot;&quot;&quot;</span>
    index <span style="color: #333333">=</span> <span style="color: #333333">-</span><span style="color: #0000DD; font-weight: bold">1</span>
    <span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #007020">len</span>(arr)):
        <span style="color: #008800; font-weight: bold">if</span> arr[i] <span style="color: #333333">==</span> val:
            index <span style="color: #333333">=</span> i
            <span style="color: #008800; font-weight: bold">break</span>
    <span style="color: #008800; font-weight: bold">return</span> index
</pre></td></tr></table></div>

## Code Block 12
```
# Pull request 5
int_arr = [1, 2, 5, 2, 10, 45, 9, 100]

def print_sorted(arr):
    """Prints the items in the array after sorting"""
    arr.sort()
    for num in arr:
        print(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7
8</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Pull request 5</span>
int_arr <span style="color: #333333">=</span> [<span style="color: #0000DD; font-weight: bold">1</span>, <span style="color: #0000DD; font-weight: bold">2</span>, <span style="color: #0000DD; font-weight: bold">5</span>, <span style="color: #0000DD; font-weight: bold">2</span>, <span style="color: #0000DD; font-weight: bold">10</span>, <span style="color: #0000DD; font-weight: bold">45</span>, <span style="color: #0000DD; font-weight: bold">9</span>, <span style="color: #0000DD; font-weight: bold">100</span>]

<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">print_sorted</span>(arr):
    <span style="color: #DD4422">&quot;&quot;&quot;Prints the items in the array after sorting&quot;&quot;&quot;</span>
    arr<span style="color: #333333">.</span>sort()
    <span style="color: #008800; font-weight: bold">for</span> num <span style="color: #000000; font-weight: bold">in</span> arr:
        <span style="color: #008800; font-weight: bold">print</span>(num)
</pre></td></tr></table></div>
