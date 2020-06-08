# Exploration: CI in This Course
## Code Block 1
```
def my_func():
	return "Hello World"
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">my_func</span>():
	<span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&quot;Hello World&quot;</span>
</pre></td></tr></table></div>

## Code Block 2
```
import unittest
import task


class TestCase(unittest.TestCase):

	def test1(self):
        expected = "Hello World"
        self.assertEqual(task.my_func(), expected)

    def test2(self):
        expected = "Goodbye World"
        self.assertNotEqual(task.my_func(), expected)


if __name__ == '__main__':
    unittest.main()
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
17</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">import</span> <span style="color: #0e84b5; font-weight: bold">unittest</span>
<span style="color: #008800; font-weight: bold">import</span> <span style="color: #0e84b5; font-weight: bold">task</span>


<span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">TestCase</span>(unittest<span style="color: #333333">.</span>TestCase):

	<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test1</span>(<span style="color: #007020">self</span>):
        expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&quot;Hello World&quot;</span>
        <span style="color: #007020">self</span><span style="color: #333333">.</span>assertEqual(task<span style="color: #333333">.</span>my_func(), expected)

    <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">test2</span>(<span style="color: #007020">self</span>):
        expected <span style="color: #333333">=</span> <span style="background-color: #fff0f0">&quot;Goodbye World&quot;</span>
        <span style="color: #007020">self</span><span style="color: #333333">.</span>assertNotEqual(task<span style="color: #333333">.</span>my_func(), expected)


<span style="color: #008800; font-weight: bold">if</span> __name__ <span style="color: #333333">==</span> <span style="background-color: #fff0f0">&#39;__main__&#39;</span>:
    unittest<span style="color: #333333">.</span>main()
</pre></td></tr></table></div>
