# Create Site Manually
* BM > Administration > Sites > Manage Sites > New
* Configuration
  * General
    * Name:
    * Time Zone
    * Default Currency
    * Taxation
    * Customer List
  * Setings
    * Cartriges
  * Cache
    * TTL: 0
    * Enable Page Caching: UnCheck Enable Page Caching
  * Site Status
    * Site Status: Online (Protected)
    * password
# Create a Catalog
* BM > Merchant Tools > Catalog > New
## Add new Catalog
* Configuration
  * General
    * CatalogID: click "apply"
  * Site Assignments
    * Select the site
    * Click Apply
* Once done, click `"<<Back to List"`
## Add Catalog Categories
* BM > Merchant Tools > Catalogs > Select the catalog > Categories > New
* Configuration
  * General
    * Category ID
    * Enable Online
    * Click Apply
    * Name
    * Click Apply
  * Category Attributes
    * Show in Menu Navigation: Check
    * Click Apply
  ## Add Products
  * BM > Merchant Tools > Products > New
  * Configuration
    * General
      * ID
      * Catalog: Select the catalog
      * Online: Yes
      * Click Apply
    * Categories
      * Click "Edit categories"
      * Select the category from list
      * Click Apply
  * Click "UnLock"
## Add Price Book
* BM > Merchant Tools > Price Books > New
* Configuration
  * General
    * ID
    * Name
    * Check "Activated"
    * Currency
    * Click Apply
  * Site Assignments
    * Select the site
    * Click Apply
## Add Inventory to the product
* BM > Merchant Tools > Products > Select the product > Inventory
* Select the Inventory
* Click "Create"
* Configuration
  * General
    * Allocation
    * Click "Create"
    * Review other configurations
    * Click "Apply"
## Link Price Books in Product
* BM > Merchant Tools > Products > Select the product > Pricing > New
* Select the Price Books
* Click "Assign"
* Enter price Info
* Enter Price Table
* Click "Apply"

## Add images to product
* First step is to upload the image
* Navigate to BM > Administration > Development Setup > Catalog > Click the catalog link
* Create the folder "default"
* Create another subfolder "large","medium",...
* Upload the file to respective folder
* Configure the image to product
* BM > Merchant Tools > Products > Select the product > General
* Click "Lock" to perform the change
* Search for images, Click Edit
* select the file and drag and drop the file
* Click "Save"
