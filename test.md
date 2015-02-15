---
layout: page
title: test
---


<pre><code id="code-arendelle" class="arendelle">[ 10 , pr ]</pre></code>

<pre><code id="code-arendelle" class="arendelle">[ 23 , pr ]</pre></code>

<script type="text/javascript">
	var highlight_elements = document.getElementsByClassName('arendelle');
	for (var i = 0; i < highlight_elements.length; ++i) {
    	var item = highlight_elements[i];  
    	item.innerHTML = highlight(item.innerHTML);
	}
</script>