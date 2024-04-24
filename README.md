# Wiki-Scraping-and-Knowledge-Graphs
Code is modified from Chris Thorton from https://towardsdatascience.com/auto-generated-knowledge-graphs-92ca99a81121

First we want to scrape the wikipedia page with:
wiki_data = wiki_page('PAGE NAME') , this works for any wikipedia page

Then retrieve our entity pairs with
pairs = get_entity_pairs(wiki_data.loc[0,'text'])

Create full knowledge graph with
draw_kg(pairs)

Finally draw a filtered knowledge graph with
filter_graph(pairs, 'CHOSEN NODE')

optional:
feel free to play with the layout on this line
 layout = (nx.planar_layout(k_graph))
