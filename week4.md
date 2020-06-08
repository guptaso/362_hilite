# Exploration White Box Testing
## Code Block 1
```
def mystery_func3(a,b):
	if a or b:
		print('At least one is True')
	else:
		print('At least one is False')
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">mystery_func3</span>(a,b):
	<span style="color: #008800; font-weight: bold">if</span> a <span style="color: #000000; font-weight: bold">or</span> b:
		<span style="color: #008800; font-weight: bold">print</span>(<span style="background-color: #fff0f0">&#39;At least one is True&#39;</span>)
	<span style="color: #008800; font-weight: bold">else</span>:
		<span style="color: #008800; font-weight: bold">print</span>(<span style="background-color: #fff0f0">&#39;At least one is False&#39;</span>)
</pre></td></tr></table></div>

# HW2
```
def contrived_func(val):
    # This function serves no logical purpose
    # DO NOT try to make sense of it!
    # Just make sure your tests cover everything requested
    # val is a numerical value
    if val < 150 and val > 100:
        return True
    elif val * 5 < 361 and val / 2 < 24:
        if val == 6:
            return False
        else:
            return True
    elif (val > 75 or val / 8 < 10) and val**val % 5 == 0:
        return True
    else:
        return False
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
16</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">contrived_func</span>(val):
    <span style="color: #888888"># This function serves no logical purpose</span>
    <span style="color: #888888"># DO NOT try to make sense of it!</span>
    <span style="color: #888888"># Just make sure your tests cover everything requested</span>
    <span style="color: #888888"># val is a numerical value</span>
    <span style="color: #008800; font-weight: bold">if</span> val <span style="color: #333333">&lt;</span> <span style="color: #0000DD; font-weight: bold">150</span> <span style="color: #000000; font-weight: bold">and</span> val <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">100</span>:
        <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">True</span>
    <span style="color: #008800; font-weight: bold">elif</span> val <span style="color: #333333">*</span> <span style="color: #0000DD; font-weight: bold">5</span> <span style="color: #333333">&lt;</span> <span style="color: #0000DD; font-weight: bold">361</span> <span style="color: #000000; font-weight: bold">and</span> val <span style="color: #333333">/</span> <span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">&lt;</span> <span style="color: #0000DD; font-weight: bold">24</span>:
        <span style="color: #008800; font-weight: bold">if</span> val <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">6</span>:
            <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">False</span>
        <span style="color: #008800; font-weight: bold">else</span>:
            <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">True</span>
    <span style="color: #008800; font-weight: bold">elif</span> (val <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">75</span> <span style="color: #000000; font-weight: bold">or</span> val <span style="color: #333333">/</span> <span style="color: #0000DD; font-weight: bold">8</span> <span style="color: #333333">&lt;</span> <span style="color: #0000DD; font-weight: bold">10</span>) <span style="color: #000000; font-weight: bold">and</span> val<span style="color: #333333">**</span>val <span style="color: #333333">%</span> <span style="color: #0000DD; font-weight: bold">5</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">0</span>:
        <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">True</span>
    <span style="color: #008800; font-weight: bold">else</span>:
        <span style="color: #008800; font-weight: bold">return</span> <span style="color: #007020">False</span>
</pre></td></tr></table></div>

## Code Block 2
```
if __name__ == '__main__':
    unittest.main()
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">if</span> __name__ <span style="color: #333333">==</span> <span style="background-color: #fff0f0">&#39;__main__&#39;</span>:
    unittest<span style="color: #333333">.</span>main()
</pre></td></tr></table></div>
