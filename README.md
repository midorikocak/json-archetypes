#Data Archetypes

###Open-source JSON standards for common types of data.
  
>**Data should be able to flow fast and freely between multiple applications...**  
>To achieve this, we need standard formats for data.  If data does not change shape, it's easier for developers to build applications that work with it, and it allows users to import pre-existing data into those applications, increasing productivity of their data.

Given the popularity of JSON, each Data Archetype has been modeled in [JSON Schema](http://json-schema.org "http://json-schema.org") format.  Data Archetypes focus on containing only the essential properties/attributes that define and differentiate types of data.

This project was started for [Servant - The Content Management Ecosystem](http://servant.co), which allows Users to host Data Archetypes in the cloud and import them into applications that work with the Archetypes.  Servant also splits the hosting revenue of its users with every applications that integrates with it.  Hosting user data separate from applications that use it, and keeping that data in standard formats are major steps toward a more liquid web :)

Feel free to contribute to the Data Archetypes!

##F.A.Q.
###As a Developer, how can I store extra data in each Archetype (e.g. SEO data)?
95% of the time, developers want to add extra data/properties to the Archetypes which are only relevant to their particular applications.  However, the Data Archetypes must be kept lean and comprehensible for the sake of speed and ease-of-use in all scenarios.  For instance, what use would a mobile application have for SEO data if SEO data is stored in each Archetype?

There are infinite use cases for each Data Archetype.  Therefore, storing custom data for each use case would result in infinite bloat.

Instead, we recommend two approaches: 

**Extend The Data Within Your Own Application:**  Set up a database and use it to store the extra data and the Data Archetype ID to which it corresponds. 

**Propose Changes:**  If you think your extra data would suit many use-cases, propose adding it in the Issues area.

###As a User, how can I store extra data in each Archetype (e.g. obscure product details)?
Data Archetypes aren't going to be perfect for everyone.  But don't let the perfect be the enemy of good.  Occasionally, you may not be able to find room to squeeze in obscure details.  On the other hand, Data Archetypes radically increase distribution and use of your data.  Yes, you may miss a small detail, but more importantly you will be able to show and use your data EVERYWHERE.




** Servant (http://servant.co) hosts these Data Archetypes in the cloud on behalf of users and splits its hosting revenue with developers who build applications that use Data Archetypes.