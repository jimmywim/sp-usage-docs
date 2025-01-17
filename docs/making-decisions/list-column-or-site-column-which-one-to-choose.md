# List columns or Site columns: Which one to choose?

We have two (2) types of columns in SharePoint:

- List columns
- Site columns

One is created at the list/library level (_list columns_), and the other one at the site level (_site columns_).

From a _functionality_ perspective, they do the exact same thing. From a _reusability_ perspective, not so much.

## List columns

If we take the example of SharePoint Online, we can now [create a column in a list or document library](https://support.office.com/en-us/article/create-a-column-in-a-sharepoint-list-or-library-2b0361ae-1bd3-41a3-8329-269e5f81cfa2) very easily. Hover between 2 columns, click on the "*+*" sign, and create your column.  

But by doing that, the column will only be created at the list/library level, and therefore, be of type _List column_.
  
#### What does this mean?

It means that your column will only be available to that particular list/library, and _not_ outside that boundary. If you wish to use that column outside of that list/library, you will have to recreate it at the new location. 

Which brings us to Site columns!

## Site columns

As we've seen above, list columns are easy to create, but live in a "container" which is the list/library you create(d) it within.  

_Site columns_ on the other hand, are created at the site level, and available to reuse _from_ the site they're created in (as the starting point).  

#### What does this mean?

Well, this means that if you create a site column at the root of your site collection, the column will be available throughout the entire site collection. <br>
If you create a site column at the subsite level, this column will only be available for the subsite itself, and every other subsite(s) underneath. But not above.<br>

Site columns are "shared" between sites, but only hierachically.

## So which one should you choose?

If you're sure that the column will only need to be used/created in a particular list or library, then a _list column_ is easy and quick.<br>

If you're looking for reusability across list/library boundaries, then create a _site column_.

---

**Principal author**: Veronique Lengelle, MVP

**LinkedIn**: https://www.linkedin.com/in/veronique-lengelle-48a71b31/

**Blog**: https://veronicageek.com

**Original post**: https://veronicageek.com/sharepoint/sharepoint-2013/list-columns-or-site-columns-in-sharepoint/2018/04/
