# Catalog and Categories
 * Collection of product definition, category definitions and images.
  * 1 catalog per site
   * Example-1:
>           Storefront
>               ^
>               |
>            Catalog A
>               ^
>               |
>      +------------+-------------+
>      |                          |
>      Categories                Products
>      + TV                      + PN001
>      + Audio                   + PN002
>      + Electronics

   * Example-2:
>        Storefront
>            ^
>            |
>        Catalog A            Catalog B
>            ^                   ^
>            |                   |
>      +---------+----------+  +-----+-------+
>      |                    |  |             |
>     Categories          Products      Class Categories
>      + TV                + PN001       + BMEcat 001
>      + Audio             + PN002       + BMEcat 002
>      + Electronics

  ## Creating and Assigning Catalogs
  * Products and Catalogs > Catalogs
  * Click "New"
  * On General tab, following are specification
    * Name
    * CatalogId
    * Description
    * Language
  * Click "Apply"
  ## Assigning Catalogs to Sites
  * Products and Catalogs > Catalogs
  * Click "Edit" and then select "Site Assignments" tab
  * Checkbox the site and click ***"Apply"***
  ## Catalog-level Search Refinement
  * Products and Catalogs > Catalogs > [Your_Catalog]
  * Click "Edit"
  * On "Search Refinement Defintions" tab for a category
  * Click "New"
  * Specify the refinement type.
  * Click "Apply"
# Categories
  * Product and Catalogs > Catalogs
## Copy Categories
  * 2 options for copy
    * **Shallow Copy** - Copies entire definition except sub-categories, attributes and search refinements.
    * **Deep Copy** - Copies entire definition including the sub-categories.
## Editing Categories
  * Edit the sub-categories
  * Edit the Category definition
  * View the category in the store front
  * Sort the list of categories as they appear in store front
  * Add or Remove category links
  * Assign or unassign products to the categories
## Linking Categories
  * Products and Catalogs > Catalogs
  * Select the catalog to view the list of categories
  * Click "New" in Categories Link section
  * Click "Next>>"
    * Accessories - Complimentary product
    * Cross-selling - related products
    * Up-selling - Higher-value products
    * Spare parts - spare parts of products
    * Other - Categories without a specific link classification
  * Select catalog from list and click "Next>>"
##  Modifying Category Display order
  * Select the category
  * Move the order using up or down in the sorting column
## Managing Category Search Engine Optimization Attributes
# Products
## Bookmarklet
  * Administration > Site Development > Development setup
  * Drag and drop "Show site Preview Information" link onto browser toolbar
## Product Category Assignments
  * Products > Product > Categories
  * Options available
    * Edit All
    * Edit Selected
    * Assign
    * New
    * Copy
    * Delete
# Product Set Tab
  ## Product Attribute Definitions
  * Merchant Tools > Product and Catalogs > Catalogs > Product Attribute Definitions
  ## Adding Product Attributes to an Attributes Group
  * Products and Catalogs > Catalogs > CatalogId - Edit > Product Attribute Definitions > Select Product Attribute > Edit
  ## Assigning Product to a Category
  * Products and Catalogs > Catalogs > {CatalogId} > {Category}
  * From category page, select products and click "Assign"
  ## Managing Product-Category Assignments
  ## Assigning Product Default Categories
  * Products and Catalogs > Products > Categories
# Product Locking
  * Time during which the product cannot be edited by others
  * Merchant Tools > Site Preferences > Locking
# Product sets
  * To represent group of products for presentation in storefront.
  * Like, presenting entire outfit for consideration, from which customer chooses pieces to purchase individually.
# Product Option Model
  * Feature allowing to customize the product like different size of hard disk and warranty options.
  ## Managing Product Option Model
  * Create attributes in system object editor, Administration > Site Development > System Objects
  * Create global options, Products and Catalogs > Product Options.
  ## Creating and assigning options
  * Products and Catalogs > Products > {Product} > Options tab
    ### Create local option
    * Click "Lock", "New"
    * Supply Name and ID and then click "Apply"
    * Specify product options, click "Apply" (_For sorting use arrows_)
    * Click "Apply"
  ## To edit a product option
  * Click on the link of that option to open the product option value editor
  ## Adding a new local option values
  * Use "New Value" in the value list
  * Supply, ID, Value, Option prize and optional SKU and click "Apply"
  * Use the currency drop-down control to change the input currency and to enter prices in a different currency.
  ## Shared product options
  * For Global production options, navigate to Products and Catalogs > Product Options
  * Select the catalog
  * It will display all shared product options
  * Click New to open shared options
  * Click [...] from list of previously created attributes
  * Click Apply
# Product Variations
  * Product variation in some attributes like color or size etc.
  * PVA (Product Variation Attribute)
  ## Managing Product Variations
  * Products and Catalogs > Products > [your product] > variations tab
  * Variation attributes can be Local or Shared
    ### Variation Attributes
    * This allows you to select and maintain the variable attributes of the variation. Ex: Color and Size.
    ### Variation Products
    * This allows to create the combination of Variation Attributes and Products.
    * For example, Phone (product) with different Colors (Black, Sliver, etc)
  ## Viewing Product Variations in Storefront
# Importing and Exporting
 * Products and Catalogs > Import & Export
# Pricing and Price Books
  * Price of a products are managed using price book
  * Price book contain price of products based on currency.
  ## Managing price books and sites
  * Relationship between price books and site is N to N
  ## Nested pricing
  * Price books can be nested using "Based On" option from price books
  ## Creating Price Books and Price Tables
  * Products and Catalogs > Price Books
  * Click New
  * On price book detail page, General Information tab
    * ID
    * Activated
    * Name
    * Description
    * Currency
    * Based On
    * Valid From
    * Valid To
  * Click Apply
  * Select Price Definitions tab to populate price books with prices.
  ## Creating prices in Price Book
  * Products and Catalogs > Price Books > Price Definitions
  ## Making price book - site assignment
  * Products and Catalogs > Price Books > Site Assignments tab
  * Select the site and Click "Apply"
  ## Assigning Price Books to Source Code
  * Online Marketing > Source-Code Groups > Price Books
  ## Product Price Indexing
# Price Lookup
  * Mechanism determines the best price (lowest price) for that quantity.
# Recommendation
# Inventory