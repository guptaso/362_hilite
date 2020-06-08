# Exploration: Unit Testing
## Code Block 1
```
def avgList(list):
	"""
	Averages the elements in a list
	:arg list: list of numbers
	:returns: the average of the list
	"""
	sum = 0
	for num in list:
		sum = sum + num
	return int(sum) / len(list)
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
10</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">avgList</span>(<span style="color: #007020">list</span>):
	<span style="color: #DD4422">&quot;&quot;&quot;</span>
<span style="color: #DD4422">	Averages the elements in a list</span>
<span style="color: #DD4422">	:arg list: list of numbers</span>
<span style="color: #DD4422">	:returns: the average of the list</span>
<span style="color: #DD4422">	&quot;&quot;&quot;</span>
	<span style="color: #007020">sum</span> <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">0</span>
	<span style="color: #008800; font-weight: bold">for</span> num <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">list</span>:
		<span style="color: #007020">sum</span> <span style="color: #333333">=</span> <span style="color: #007020">sum</span> <span style="color: #333333">+</span> num
	<span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">int</span>(<span style="color: #007020">sum</span>) <span style="color: #333333">/</span> <span style="color: #007020">len</span>(<span style="color: #007020">list</span>)
</pre></td></tr></table></div>

## Code Block 2
```
class TestAvgList(unittest.TestCase):
	pass
  ```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestAvgList</span>(unittest<span style="color: #333333">.</span>TestCase):
	<span style="color: #008800; font-weight: bold">pass</span>
</pre></td></tr></table></div>

## Code Block 3
```
import unittest
from unit_testing import avgList

class TestAvgList(unittest.TestCase):
	pass
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">import</span> <span style="color: #0e84b5; font-weight: bold">unittest</span>
<span style="color: #008800; font-weight: bold">from</span> <span style="color: #0e84b5; font-weight: bold">unit_testing</span> <span style="color: #008800; font-weight: bold">import</span> avgList

<span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestAvgList</span>(unittest<span style="color: #333333">.</span>TestCase):
	<span style="color: #008800; font-weight: bold">pass</span>
</pre></td></tr></table></div>

## Code Block 4
```
def test1(self):
	list = [1,2,3]
	expected = 2
	self.assertEqual(avgList(list), expected, msg='avgList({})'.format(list))
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">list</span> <span style="color: #333333">=</span> [<span style="color: #0000DD; font-weight: bold">1</span>,<span style="color: #0000DD; font-weight: bold">2</span>,<span style="color: #0000DD; font-weight: bold">3</span>]
	expected <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">2</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(avgList(<span style="color: #007020">list</span>), expected, msg<span style="color: #333333">=</span><span style="background-color: #fff0f0">&#39;avgList({})&#39;</span><span style="color: #333333">.</span>format(<span style="color: #007020">list</span>))
</pre></td></tr></table></div>

## Code Block 5
```
def test2(self):
	list = []
	expected = 0
	self.assertEqual(avgList(list), expected, msg='avgList({})'.format(list))
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test2</span>(<span style="color: #007020">self</span>):
	<span style="color: #007020">list</span> <span style="color: #333333">=</span> []
	expected <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">0</span>
	<span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(avgList(<span style="color: #007020">list</span>), expected, msg<span style="color: #333333">=</span><span style="background-color: #fff0f0">&#39;avgList({})&#39;</span><span style="color: #333333">.</span>format(<span style="color: #007020">list</span>))
</pre></td></tr></table></div>

## Code Block 6
```
if __name__ == '__main__':
	unittest.main(verbosity=2)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">if</span> __name__ <span style="color: #333333">==</span> <span style="background-color: #fff0f0">&#39;__main__&#39;</span>:
	unittest<span style="color: #333333">.</span>main(verbosity<span style="color: #333333">=</span><span style="color: #0000DD; font-weight: bold">2</span>)
</pre></td></tr></table></div>
