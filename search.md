---
title: Search
layout: default
permalink: /search/
tipue_search_active: true
exclude_from_search: true
---
<script src="{{site.github.url}}/assets/scripts/jquery.min.js"></script>
<script src="{{site.github.url}}/assets/search/tipuesearch_content.js"></script>
<script src="{{site.github.url}}/assets/search/tipuesearch_set.js"></script>
<script src="{{site.github.url}}/assets/search/tipuesearch.js"></script>

## Search Form

<form action="{{site.github.url}}{{ page.url }}" style="display: flex;">
    <input type="text" name="q" id="tipue_search_input" pattern=".{3,}" title="At least 3 characters" required style="margin-right: 10px">
    <button class="button button--icon" type="submit">
    <span>{% include icon.html name="search"%}</span>&nbsp;<span>Search</span>
    </button>
</form>

## Search Results

<div id="tipue_search_content"></div>

<script>
$(document).ready(function() {
  $('#tipue_search_input').tipuesearch();
});
</script>
