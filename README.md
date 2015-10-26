# MongoViews
it maps on the fly, projecting a different schema onto a document.

The intent is to extract weird nested data from remote APIs, and map it to a better model that represents our mental model of it. It can be queried with the better model, too. It’s mostly for read-only queries, although i made it writable, too. 

Other systems stash raw data into the collection, and then we can read it with a nicer interface. And when those systems add or even update the data, all changes are seen in the model, too, because it’s just a mapping. Woot. 

