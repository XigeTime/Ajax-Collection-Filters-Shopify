# Shopify Section for Collection Filters 
A section block for Shopify that adds some nice select boxes for filtering collections by tags.

Allows for separating tag groups into separate select boxes for a clean look.

Ajaxify setting so customers can browse without having the page refresh.

Filters are based on Shopifys default filter system which uses tags, examples include price filter, type filter, brand filter, colours, sizes and many more.

Original by <b>Nitin Sharma</b> forked by <b>Harry K (xigetime)</b>

# Usage
1. Simply drop the <b>collection-filters-section.liquid</b> file into your sections directory.
2. In your <b>collection.liquid</b> template, add the following to include the section:
`{% section 'collection-filters-section' %}`
3. In your Shopify Admin dashboard, navigate to Themes > Your Theme > Customise > Then open a collection page and you should see the filters section ready to be configured!

# Settings
1. <b>Enable tag filtering</b>: Enables/disables the collection filters from within the admin
2. <b>Filter Type</b>: Choose whether you would like to filter by any available tags, or a specific group of tags.
3. <b>Groups to use in filter</b>: If groups is selected for filter type, here seperated by a comma you can specifiy each filter group.
4. <b>Ajaxify Filters</b>: Turn this on to fetch the new products/pages via Ajax.
5. <b>Product container class or id</b>: The products container element selector, everything inside this element will be replaced with the new pages products.
6. <b>Pagination container class or id</b>: The paginations container element selector, we need to fetch the pagination, otherwise when they go to the next page they will loose their filters.

# Group tag format
Group tags, are product tags and should be formatted like so: <b>Group<span style="color:red">:</span>Value</b>

Examples: <b>Brand:Nike</b> - <b>Size:L</b> - <b>Vendor:Me</b> - <b>Price:Under 10</b>