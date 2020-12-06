 # Wine Categorization

It is useful to bucket wines into different categories. Too often, categorization systems that exist for wine are muddled and inconsistent. 

We can categorize wine along the following dimensions:

- Category
- Region
- Grape Type (Variety and Clone)
- Single-Varietal or Blend
- Wine Style

_________________________
### Category

The highest-level bucket we can divide wines into is categories. This is synonymous with the 'type' of wine: 
- Red
- White
- Rosé
- Orange
- Sparkling
- Fortified/Dessert

Here, 'Sparkling' takes precedence as a category over 'White' or 'Rosé' (e.g. a Sparkling Rosé would fall under the 'Sparkling' category).

________________________
### Region

Every wine can be assigned to a single region. This region provides an indication of where the grapes have been grown. 

Some wines are made with grapes from a single plot inside a specific vineyard. Other wines are made with grapes from a number of different vineyards that can be located in different AVA's (US), counties, states or even countries. 

There are specific labeling rules for what location(s) can be attributed to a wine. These rules differ around the world. For example: a wine made with grapes from all over California will be labeled 'California'. A wine made with grapes that come from a specific vineyard in Rutherford can be labelled 'Rutherford'. 

Rather than coming up with a full list of all these rules, we have built a hierarchical taxonomy consisting of the possible locations that can be attributed to a wine. 

________________________
### Grape Type (Variety and Clone)

Every (grape) wine is made with one or more grape varieties. Unless a wine is a field blend, or a proprietary combination of different varieties, it can be broken out into its constituent components.

Biologically, grape variety (or cultivar) is a sub-level underneath species. Most grape varieties belong to the 'Vitis Vinifera' species, although there are exceptions.

One thing to note is that grape varieties can have many synonyms. Pinot Grigio, for instance, is called Pinot Gris in France and Grauburgunder in Germany. We are yet to add a mapping of these synonyms. 

Clones describe variations within a grape variety that are cultivated through a process called grafting. We won't go into detail on this here - what is important to know is that a grape variety can have multiple different clones. 

Clones are sometimes named using the FPS naming convention, known for its use by UC Davis (https://fps.ucdavis.edu/fgrvarieties.cfm). Other times, clones are named using the ENTAV-INRA standards (http://www.entav-inra.fr/en/trade-mark/). 

In the interest of consistency, we have chosen to go with the FPS standards, but would like to supplement this with a mapping to the ENTAV-INRA names also.


________________________
### Single-Varietal or Blend

Every wine consists of a single-varietal or is a blend of different varieties. We can label a wine accordingly.

A complicating factor here is labeling standards. In most of the US, if a wine consists of at least 75% one grape variety, it can be labeled as a single-varietal wine. In Oregon, this is 90%. The percentages are yet different in other places around the world. 

Rather than listing out all of the rules here, it is sufficient to mark a wine as single-varietal or a blend. 


_________________________
### Wine Style

'Wine Style' is a term that is used to mean many different things. We would like to propose that this term be standardized to mean the *style in which a wine has been produced, often driven by a varietal and/or region.* 

We can consider wine style as a combination between Category, Single-Varietal/Blend and Grape Type - plus a stylistic factor.

Let us illustrate through an example: Chardonnay is made in different styles around the world. Three of the most well-known styles are:

1. California-style Chardonnay
2. Chablis-style Chardonnay
3. Burgundy-style Chardonnay

Any single-varietal Chardonnay that is produced around the world will fall into one of these three styles, or can alternatively just be assigned a style equal to its grape variety: Chardonnay. 

For blends, wine style is a little different - a (dry) blend of Semillon and Sauvignon Blanc is likely to be a Bordeaux-style White Blend. If it has not been made in the Bordeaux style, it can be assigned a catch-all wine style: 'White Blend'. 

A similar mechanism can be used as a catch-all for wine styles in single-varietal wines. It would be overkill to assign a different wine style to every single grape variety. Grape varieties that are less common can be assigned a wine style such as 'Other Red' or 'Other White'. 