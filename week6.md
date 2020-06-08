# Exploration: Test Driven Development
## Code Block 1
```
def test1(self):
	input = 1
	expected = '1'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">1</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;1&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 2
```
def fizz_buzz(num):
	return '1'
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;1&#39;</span>
</pre></td></tr></table></div>

## Code Block 3
```
def test2(self):
	input = 2
	expected = '2'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test2</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">2</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;2&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 4
```
def fizz_buzz(num):
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>

## Code Block 5
```
def test3(self):
	input = 3
	expected = 'fizz'
	self.assertTrue(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test3</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">3</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertTrue(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 6
```
def fizz_buzz(num):
	if num == 3:
		return 'fizz'
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">3</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>

## Code Block 7
```
def test5(self):
	input = 5
	expected = 'buzz'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test5</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">5</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 8
```
def fizz_buzz(num):
	if num == 3:
		return 'fizz'
	if num == 5:
		return 'buzz'
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">3</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">5</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>


## Code Block 9
```
def test6(self):
	input = 6
	expected = 'fizz'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test6</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">6</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 10
```
def fizz_buzz(num):
	if num % 3 == 0:
		return 'fizz'
	if num == 5:
		return 'buzz'
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">3</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">5</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>

## Code Block 11
```
def test10(self):
	input = 10
	expected = 'buzz'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test10</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">10</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 12
```
def fizz_buzz(num):
	if num % 3 == 0:
		return 'fizz'
	if num % 5 == 0:
		return 'buzz'
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">3</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">5</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>

## Code Block 13
```
def test15(self):
	input = 15
	expected = 'fizzbuzz'
	self.assertEqual(fizz_buzz(input), expected)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test15</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">input</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">15</span>
	expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&#39;fizzbuzz&#39;</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(fizz_buzz(<span style="color: #007020">input</span>), expected)
</pre></td></tr></table></div>

## Code Block 14
```
def fizz_buzz(num):
	if num % 3 == 0 and num % 5 == 0:
		return 'fizzbuzz'
	if num % 3 == 0:
		return 'fizz'
	if num % 5 == 0:
		return 'buzz'
	return str(num)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6
7
8</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">fizz_buzz</span>(num):
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">3</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span> <span style="color: #000000; font-weight: bold">and</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">5</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizzbuzz&#39;</span>
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">3</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;fizz&#39;</span>
	<span style="color: #008800; font-weight: bold">if</span> num <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">5</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
		<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;buzz&#39;</span>
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">str</span>(num)
</pre></td></tr></table></div>
