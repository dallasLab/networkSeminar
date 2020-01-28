
Hello. I'm Tad, and I want to talk about global patterns of host-helminth associations. 

This work, and my interest in large scale patterns of parasite diversity, really began during my PhD, where I had the opportunity to become involved with the Macroecology of Infectious Disease Research Coordination Network. This picture was taken during our meeting at the Cary Institute in 2017. Some of the people in this picture are also in this room, and have contributed to my development as a scientist. 

One of the products of this ongoing collaborative group was a review paper describing how macroecological theory could be tested using parasite species. And one of the things that I took away from this effort was that the theory is there, but one major limitation is the availability of large scale data on host-parasite associations. 

This barrier has been slightly overcome a bit, and I want to focus on one data resource in particular, the London Natural History Museum's helminth database. This is a collection of around a quarter of a million host-helminth records obtained from primary literature (over 28k published studies). This data resource consists of over 18k unique host species and 27k unique helminth parasite species. It also has an R interface through the package helminthR, which allows users to query data from host species, helminth parasites, and locations. 

The data are georeferenced to the country level (largely, though some bodies of water are also included). 

Apart from being widespread, the London Natural History Museum's helminth database is the largest host-parasite occurrence database currently known in terms of occurrences (proportional to point size) as well as the number of unique host and parasite species, despite just being composed of helminth species.


And these data allow the large scale examination of diversity patterns at large spatial scales. If we standardize parasite diversity by host diversity (thus calculating the mean number of helminth parasites per host species), we see a pronounced spatial variability in parasite diversity after attempting to account for host diversity. But species richness is a bit of a crude estimate relative to the wealth of information we have about these host and helminth communities. 

So if we consider the similarity of communities as a function of geographic distance between pairs of sites, we see another level of variability. So species richness demonstrated some spatial variability, and now we can see that host (on the left) and helminth parasite (on the right) communities become quickly dissimilar (y axis, with large values indicating dissimilarity). This suggests that species are turning over across space fairly rapidly. 

But this belies the fact that some host and helminth parasite species appear in numerous country-level networks. This distributional map suggests that this host species could potentially appear in many different networks. 

In case anybody is wondering, this is the distributional map for the rock pigeon, but certainly other species also appear in multiple networks. 

And this leads to the question that was uncovered after these initial examinations of host and parasite diversity patterns in space, which is to what extent do host and helminth parasite species tend to serve the same role in the country-level network of host-helminth associations? We might expect that species roles would be conserved, if specialist parasite species remain specialist parasites across their spatial distribution, and the same for host species and their helminth parasite richness. 


To clarify this, and to explain how we went about quantifying species roles, we can look at this simple network of host species on the top row and helminth parasites on the bottom. The color indicates two different modules, which are estimated by an algorithm that attempts to group sets of nodes based in a way to maximize within module connections and minimize between module connections. 

And we can use individual species relative number of within module connections (here in red for the red host) ...

and between module connections (still in red), to quantify species roles. 

And this approach has been fruitfully applied by previous researchers, one of which is Pedro Jordano, who is a collaborator on this project. 

And the importance of between module and within module connections creates a 2-dimensional space where nodes can occupy. And within this space, we can quantify species roles in two ways. First, we can calculate the area enclosed for each species here (where the pink bear is an example), and compare this to a null distribution of area values. Or, in green, we can use this approach of classifying species as either module hubs, network hubs, connectors, or peripheral species. I'll briefly discuss both ways, but I'm going to spill the beans and tell you that the results are the same regardless of approach.

So we widdled down the location data to those locations which weren't ambiguous or nested within other locations, resulting in right around 100k host helminth occurrence records for a whole bunch of species. And we calculated species roles using our approaches for this whole set of almost 40k species, and examined the fraction of times that the species role in the global network considering ALL host-helminth associations matched that of each country-level subnetwork. 

It was rare that the role matched. Here, each barplot corresponds to the species role in the global network, and the x-axis is the fraction of times a given species played that part in the subnetworks. And we found, not very often. 

And the story is the same when we don't consider this global network approach, but instead create a null distribution and compare each species to some null expectation of area in this 2d "role space". Of the 40k species, only a very very small number of species had spatially conserved roles in host-helminth networks. 


This suggests that species topological role, based on how we defined species roles, is not conserved in host-helminth networks. And it emphasized something to me that I neglected as we developed this project, and that is that 

the context of the local network is important. The complex relationships between host and parasite depend on the presence of suitable host species, presence of suitable helminth parasites, and -- as we calculated species roles -- the relative associations between other host and helminth species in the network. 


Understanding how this local network context leads to spatial variation in species roles is really important, as species role estiamted from one subnetwork will likely not apply to another network. In terms of invasion biology, this would suggest that a range shifting host species that has moved into a novel host-helminth network may have a wildly different set of interactions and relative role in the alien range than in the hosts native range. Lastly, this is important when considering what sorts of relevant spatial or environmental gradients may structure the variation in species roles. 


Before I end, I'd like to thank HPC-Europa III, the grant that allowed me to work with Pedro and have access to the Barcelona supercomputer. 

And I'd also like to note that I have just begun an assistant professorship at Louisiana State University, and I would love to talk with interested graduate students and postdocs about joining the lab. It's a great university, department, and lab. 

And with that I will run off stage because I may not have time for questions. However, I will be around, and my contact information is there if we don't get a chance to interact. Thank you.






