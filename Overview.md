# Types of Instances
* Stg
* Dev
* Prod
* Sandbox
* On-demand sandbox

# what are PIG and SIG instances?
* Primary instance group
* Secondary instance group
   * 46 + 1 instances
   * 46 are sandbox instances
   * 1 demo sandbox
   * Sandbox instance will be in running state always.

# What is Realm?
* This will contain all STG, DEV, PROD and Sandbox instances.

# What is POD?
* Point of Delivery
* POD will contain multiple Realm.

# Types of Cartridges
Abbrevation | Definition
------------|--------------------
int:        | Integration
bm:         | Business Manager
bc:         | Business Component
plugin:     | Plugin
app:        | Application
lib: | ?

# Cartridge Folder Structure
* app_samplecartridge
  * cartridge
    * client
    * config
    * controllers
    * experience
    * forms
    * models
    * scripts
    * static
    * template
    * webreferences
    * app_samplecartridge.properties
  * .project
  * .tern-project
# ISML tags

# Content Asset
* What is content asset?
* How to configure a content asset?
  * Business Manager > Merchant Tools > Content > Content Asset
* Create a new content asset?
  * Business Manager > Merchant Tools > Content > Content Asset > New
* Render asset
  * `<iscontentasset aid="<ContentId>">` to render the content asset into application/page.
  * Another option to render content is by using "ContentMgr" api/class.
* Get content using API
# Content Slot
* What is content slot?
  * This will be majorly used for scheduling content dynamically like, product offer teaser.
  * Business Manager > Online Marketing > Content Slots.
* How to create new content slot
  * Use `<isslot>` tag
  * Syntax:
    * `<isslot id="id" context="global"| "category" | "folder" context-object=context-object description=description preview-url=url>`
* Types of slot
  * Global
    * Example: `<isslot id="homepage_banner" context="global" description="Home banner"/>`
  * Category
    * Example: `<isslot id="category_top_featured" context="category" context-object="${pdict.ProductSearchResult.category}" />`
  * Folder
    * Example: `<isslot id="fldr-landing-sotbanner" context="folder" context-object="${pdict.ContentSearchResult.folder}" description="Large Folder Landing Banner" />`
* How to configure content?
  * Business Manager > Merchant Tools > Online Marketing > Content Slots > Slot Configuration(s) > New
* Types of Content
  * Product
  * Category
  * Content Asset
  * HTML
  * Recommendation -> This needs explicit communication with SFCC to enable the recommendation engine.
* How to schedule a content slot?
  * 
* Create slot configuration
home -> bm -> banner
# Create a new site
## Manual approach
* BM > Administration > Manage Sites 
# Product Types
* Standard Product
* Variation Master
* Variation group
* Variation product
* Product set
* Product bundle