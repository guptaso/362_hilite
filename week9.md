# Exploration: Creating Testing Environments
## Code Block 1
```
def read_first_five(filename):
  file = open(filename, "r")
  contents = file.read()
  file.close()
  return contents[:5]
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">read_first_five</span>(filename):
  <span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(filename, <span style="background-color: #fff0f0">&quot;r&quot;</span>)
  contents <span style="color: #333333">=</span> <span style="color: #007020">file</span><span style="color: #333333">.</span>read()
  <span style="color: #007020">file</span><span style="color: #333333">.</span>close()
  <span style="color: #008800; font-weight: bold">return</span> contents[:<span style="color: #0000DD; font-weight: bold">5</span>]
</pre></td></tr></table></div>

## Code Block 2
```
file = open("temp_file", "w")
file.write("Hello World")
file.close()
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&quot;temp_file&quot;</span>, <span style="background-color: #fff0f0">&quot;w&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>write(<span style="background-color: #fff0f0">&quot;Hello World&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>close()
</pre></td></tr></table></div>

## Code Block 3
```
def test1(self):
  file = open("temp_file", "w")
  file.write("Hello World")
  file.close()
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
  <span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&quot;temp_file&quot;</span>, <span style="background-color: #fff0f0">&quot;w&quot;</span>)
  <span style="color: #007020">file</span><span style="color: #333333">.</span>write(<span style="background-color: #fff0f0">&quot;Hello World&quot;</span>)
  <span style="color: #007020">file</span><span style="color: #333333">.</span>close()
</pre></td></tr></table></div>

## Code Block 4
```
class TestCase(unittest.TestCase):
def test2(self):
file = open("temp_file", "w")
file.write("Hello World")
file.close()
...
def test1(self):
file = open("temp_file", "w")
file.write("Hello World")
file.close()
...
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
11</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestCase</span>(unittest<span style="color: #333333">.</span>TestCase):
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test2</span>(<span style="color: #007020">self</span>):
<span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&quot;temp_file&quot;</span>, <span style="background-color: #fff0f0">&quot;w&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>write(<span style="background-color: #fff0f0">&quot;Hello World&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>close()
<span style="color: #333333">...</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
<span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&quot;temp_file&quot;</span>, <span style="background-color: #fff0f0">&quot;w&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>write(<span style="background-color: #fff0f0">&quot;Hello World&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>close()
<span style="color: #333333">...</span>
</pre></td></tr></table></div>

## Code Block 5
```
class TestCase(unittest.TestCase):
def setUp(self):
file = open("temp_file", "w")
file.write("Hello World")
file.close()
def test1(self):
...
def test2(self):
...
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7
8
9</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestCase</span>(unittest<span style="color: #333333">.</span>TestCase):
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">setUp</span>(<span style="color: #007020">self</span>):
<span style="color: #007020">file</span> <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&quot;temp_file&quot;</span>, <span style="background-color: #fff0f0">&quot;w&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>write(<span style="background-color: #fff0f0">&quot;Hello World&quot;</span>)
<span style="color: #007020">file</span><span style="color: #333333">.</span>close()
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
<span style="color: #333333">...</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test2</span>(<span style="color: #007020">self</span>):
<span style="color: #333333">...</span>
</pre></td></tr></table></div>

## Code Block 6
```
class FileTests(unittest.TestCase):
  def setUp():
  ...

class DatabaseTests(unittest.TestCase):
  def setUp():
  ...
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">FileTests</span>(unittest<span style="color: #333333">.</span>TestCase):
  <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">setUp</span>():
  <span style="color: #333333">...</span>

<span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">DatabaseTests</span>(unittest<span style="color: #333333">.</span>TestCase):
  <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">setUp</span>():
  <span style="color: #333333">...</span>
</pre></td></tr></table></div>

## Code Block 7
```
class TestCase(unittest.TestCase):
  @classmethod
  def setUpClass(cls):
  ...
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestCase</span>(unittest<span style="color: #333333">.</span>TestCase):
  <span style="color: #555555; font-weight: bold">@classmethod</span>
  <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">setUpClass</span>(cls):
  <span style="color: #333333">...</span>
</pre></td></tr></table></div>

## Code Block 8
```
def tearDown(self):
  os.remove(self.filename)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">tearDown</span>(<span style="color: #007020">self</span>):
  os<span style="color: #333333">.</span>remove(<span style="color: #007020">self</span><span style="color: #333333">.</span>filename)
</pre></td></tr></table></div>

## Code Block 9
```
@classmethod
def tearDownClass(cls):
...
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #555555; font-weight: bold">@classmethod</span>
<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">tearDownClass</span>(cls):
<span style="color: #333333">...</span>
</pre></td></tr></table></div>

# Exploration: Stubs, Fakes, and Mocks
## Code Block 1
```
mock = Mock()
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1</pre></td><td><pre style="margin: 0; line-height: 125%">mock <span style="color: #333333">=</span> Mock()
</pre></td></tr></table></div>

## Code Block 2
```
mock = Mock()
# No declaration errors here!
mock.func()
mock.attr
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%">mock <span style="color: #333333">=</span> Mock()
<span style="color: #888888"># No declaration errors here!</span>
mock<span style="color: #333333">.</span>func()
mock<span style="color: #333333">.</span>attr
</pre></td></tr></table></div>

## Code Block 3
```
# We use the real datetime to get a real date object for a leap year date
leap_date = datetime.datetime(year=2020, month=1, day=1)
# Now we mock datetime so we can "highjack" it
datetime = Mock()
datetime.datetime.today.return_value = leap_date
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># We use the real datetime to get a real date object for a leap year date</span>
leap_date <span style="color: #333333">=</span> datetime<span style="color: #333333">.</span>datetime(year<span style="color: #333333">=</span><span style="color: #0000DD; font-weight: bold">2020</span>, month<span style="color: #333333">=</span><span style="color: #0000DD; font-weight: bold">1</span>, day<span style="color: #333333">=</span><span style="color: #0000DD; font-weight: bold">1</span>)
<span style="color: #888888"># Now we mock datetime so we can &quot;highjack&quot; it</span>
datetime <span style="color: #333333">=</span> Mock()
datetime<span style="color: #333333">.</span>datetime<span style="color: #333333">.</span>today<span style="color: #333333">.</span>return_value <span style="color: #333333">=</span> leap_date
</pre></td></tr></table></div>

## Code Block 4
```
mock.abs.call_count
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1</pre></td><td><pre style="margin: 0; line-height: 125%">mock<span style="color: #333333">.</span>abs<span style="color: #333333">.</span>call_count
</pre></td></tr></table></div>

## Code Block 5
```
# Displays last called arguments
mock.abs.call_args
# Displays list of all called arguments
mock.abs.call_args_list
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Displays last called arguments</span>
mock<span style="color: #333333">.</span>abs<span style="color: #333333">.</span>call_args
<span style="color: #888888"># Displays list of all called arguments</span>
mock<span style="color: #333333">.</span>abs<span style="color: #333333">.</span>call_args_list
</pre></td></tr></table></div>

## Code Block 6
```
# Displays all methods called on the Mock object
mock.method_calls
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #888888"># Displays all methods called on the Mock object</span>
mock<span style="color: #333333">.</span>method_calls
</pre></td></tr></table></div>

## Code Block 7
```
def load_file():
  content = open('temp_file.txt')
  if content.length != 0:
    return content
  return None
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">load_file</span>():
  content <span style="color: #333333">=</span> <span style="color: #007020">open</span>(<span style="background-color: #fff0f0">&#39;temp_file.txt&#39;</span>)
  <span style="color: #008800; font-weight: bold">if</span> content<span style="color: #333333">.</span>length <span style="color: #333333">!=</span> <span style="color: #0000DD; font-weight: bold">0</span>:
    <span style="color: #008800; font-weight: bold">return</span> content
  <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">None</span>
</pre></td></tr></table></div>

## Code Block 8
```
class TestCase(unittest.TestCase):
  def test_load(self):
    with patch('load_file.open') as mock_open:
      mock_open.side_effect = IOError
      with self.assertRaises(IOError):
        load_file()
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestCase</span>(unittest<span style="color: #333333">.</span>TestCase):
  <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test_load</span>(<span style="color: #007020">self</span>):
    <span style="color: #008800; font-weight: bold">with</span> patch(<span style="background-color: #fff0f0">&#39;load_file.open&#39;</span>) <span style="color: #008800; font-weight: bold">as</span> mock_open:
      mock_open<span style="color: #333333">.</span>side_effect <span style="color: #333333">=</span> <span style="color: #FF0000; font-weight: bold">IOError</span>
      <span style="color: #008800; font-weight: bold">with</span> <span style="color: #007020">self</span><span style="color: #333333">.</span>assertRaises(<span style="color: #FF0000; font-weight: bold">IOError</span>):
        load_file()
</pre></td></tr></table></div>
