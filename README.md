![json archetypes data standards](https://github.com/servant-cmes/json-archetypes/blob/master/json_archetypes_banner.png)

#JSON Archetypes

Simple, community-driven standards for popular types of data in JSON.  That is all.

These were made for [Servant](https://www.servant.co).  Servant is a personal database and these are its schemas.

Each JSON Archetype uses the [JSON Schema](http://json-schema.org "http://json-schema.org") format to describe the Archetype and its validation rules.  All of the Archetypes can be found in the `archetypes` folder.  JSON Archetypes are meant to be lean and contain only the essential properties/attributes that define and differentiate each archetype.  The challenge is to agree on what those properties/attributes are...
 
Feel free to contribute to the existing JSON Archetypes or create your own!


##Contributing
Anyone who has a JSON Archetype in mind, or wants to add to existing JSON Archetypes is free to contribute.  Just follow these steps:

 - Fork this project.
 - Clone your forked project (which should now be in your github account) to your computer.
 - Create a branch and work on it to create/modify existing JSON Archetypes
 - Try to submit pull requests for one Archetype at a time

More on how to contribute to a Github project [here](https://guides.github.com/activities/contributing-to-open-source/).

##Design Principles

 - **Shallow Architecture -**  Don't add nested objects.  Only Arrays are allowed, and if they contain objects, keep those objects small.  Shallow architecture makes the Archetypes more accessible using simpler queries that can be effectively indexed to scale well.
 - **Unique Property Names -** Every property name in an Archetype must be unique.
 - **Follow The JSON Schema Specs -** http://json-schema.org/example1.html 
 - **Copy Schema.org Schemas wherever you can -** http://schema.org 


##F.A.Q.

###How is this different from Schema.org?

JSON Archetypes are simpler versions of the schemas on schema.org.  While application developers can comprehend [the verbose, nested data architecture Schema.org uses](http://schema.org/docs/full.html "http://schema.org/docs/full.html"), it's still complex and not much fun to work with.

That said, we’ve tried to copy schema.org schemas wherever possible, as well as their property names, so there will be interoperability.  Hopefully we can evolve to further resemble schema.org in the future.

###Can I add additional properties to the Archetypes?

If you think the property is absolutely necessary, contribute to this repo :)

Keep in mind, developers mostly want to add properties to the Archetypes that are relevant only to the application they want to make.  Nothing wrong with that.  But, there are infinite use-cases for the Archetypes, and if we created Archetype properties for each use case, we’d have infinite bloat.

The solution is to make **meta** records for each Archetype record and save those meta records in your app's database.  For example, make a meta record in your database that relates to Product Archetype record with the ID 881JKS0A891.  In that meta record you can extend that product with properties like views, SEO keywords, etc.   


###As a User, how can I store extra data in each Archetype (e.g. obscure product details)?

Archetypes aren't going to be 100% perfect for everyone.  But don't let perfect be the enemy of good.  
Occasionally, you may not be able to find room to squeeze in obscure details.  On the other hand, the fixed formats of JSON Archetypes make it easy for apps to consume.  Yes, you may miss a small detail, but more importantly, you will increase distribution and overall productivity of your data by letting it be used everywhere.

###Bro, I found [this comic on XKCD](http://xkcd.com/927/) and it’s totally relevant.  Can I show it to you?

We've seen it, laughed, and moved forward.