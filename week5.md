# Exploration: Random Testing
## Code Block 1:
```
def my_abs(val):
	if(val > 0):
		return val
	else
		return -val
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">my_abs</span>(val):
	<span style="color: #008800; font-weight: bold">if</span>(val <span style="color: #333333">&gt;</span> <span style="color: #0000DD; font-weight: bold">0</span>):
		<span style="color: #008800; font-weight: bold">return</span> val
	<span style="color: #008800; font-weight: bold">else</span>
		<span style="color: #008800; font-weight: bold">return</span> <span style="color: #333333">-</span>val
</pre></td></tr></table></div>

## Code Block 2
```
for i in range(0,1000):
	val = random.randint(10000000,99999999)
	mystery_func(val)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3</pre></td><td><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">for</span> i <span style="color: #000000; font-weight: bold">in</span> <span style="color: #007020">range</span>(<span style="color: #0000DD; font-weight: bold">0</span>,<span style="color: #0000DD; font-weight: bold">1000</span>):
	val <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">10000000</span>,<span style="color: #0000DD; font-weight: bold">99999999</span>)
	mystery_func(val)
</pre></td></tr></table></div>

## Code Block 3
```
edge_cases = [7,8,9,19,20,21]
	odds = random.randint(1,10)
    if odds == 1:
		length = random.choice(edge_cases)
    else:
        length = random.randint(0,30)
```
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><table><tr><td><pre style="margin: 0; line-height: 125%">1
2
3
4
5
6</pre></td><td><pre style="margin: 0; line-height: 125%">edge_cases <span style="color: #333333">=</span> [<span style="color: #0000DD; font-weight: bold">7</span>,<span style="color: #0000DD; font-weight: bold">8</span>,<span style="color: #0000DD; font-weight: bold">9</span>,<span style="color: #0000DD; font-weight: bold">19</span>,<span style="color: #0000DD; font-weight: bold">20</span>,<span style="color: #0000DD; font-weight: bold">21</span>]
	odds <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">1</span>,<span style="color: #0000DD; font-weight: bold">10</span>)
    <span style="color: #008800; font-weight: bold">if</span> odds <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">1</span>:
		length <span style="color: #333333">=</span> random<span style="color: #333333">.</span>choice(edge_cases)
    <span style="color: #008800; font-weight: bold">else</span>:
        length <span style="color: #333333">=</span> random<span style="color: #333333">.</span>randint(<span style="color: #0000DD; font-weight: bold">0</span>,<span style="color: #0000DD; font-weight: bold">30</span>)
</pre></td></tr></table></div>
