<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Person</span>:
    <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">__init__</span>(<span style="color: #007020">self</span>, first_name<span style="color: #333333">=</span><span style="background-color: #fff0f0">&quot;John&quot;</span>, last_name<span style="color: #333333">=</span><span style="background-color: #fff0f0">&quot;Doe&quot;</span>):
        <span style="color: #007020">self</span><span style="color: #333333">.</span>first_name <span style="color: #333333">=</span> first_name
        <span style="color: #007020">self</span><span style="color: #333333">.</span>last_name <span style="color: #333333">=</span> last_name

    <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">get_name</span>(<span style="color: #007020">self</span>):
        <span style="color: #008800; font-weight: bold">return</span> <span style="background-color: #fff0f0">&#39;{0} {1}&#39;</span><span style="color: #333333">.</span>format(<span style="color: #007020">self</span><span style="color: #333333">.</span>first_name, <span style="color: #007020">self</span><span style="color: #333333">.</span>last_name)

    <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">set_first</span>(<span style="color: #007020">self</span>, first_name):
        <span style="color: #007020">self</span><span style="color: #333333">.</span>first_name <span style="color: #333333">=</span> first_name

    <span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">set_last</span>(<span style="color: #007020">self</span>, last_name):
        <span style="color: #007020">self</span><span style="color: #333333">.</span>last_name <span style="color: #333333">=</span> last_name
</pre></div>
