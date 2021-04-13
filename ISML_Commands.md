# ISML
 * Internet store markup Language
 * Used for presentation logic
 * ISML templates can contain
   * ISML tags
   * Plain HTML
   * Javascript
# ISML Elements
 * ISML Tags starts with "is"
   * Example: `<isinclude> <isprint>`
 * ISML expressions are based on Demandware script
   * ${Expression}
   * Example: 
     * ${pdict.Product.UUID}
     * ${pdict.Product.getLongDescription() != null}
# Commands
## Reusability with <isinclude>
* There are 2 types of includes
  * Local include
  * Remote include
### Local Include
* Includes code from another template within same source code
* Maximum include depth for template is 10
* **Syntax**
```
<isinclude 
    (template = (<template identifier> | <expression>))
    (url = (<URL> | <expression>))>
```
* **Example**
```
<isinclude template="report/report.isml">
```
### Remote Include
* This command will include the content of the given URL, typically a URL from the same server
* Maxium include depth for template is 16
* **Syntax**
```
<isinclude url="${URLUtils.url('PipelineName-StartNode')}">
```
* **Example**
```
<isinclude url="${URLUtils.url('search-show')}">
```
## Resuability with <ismodule>
* `<ismodule>` tag is used to declare custom tags in ISML templates.
* **Syntax**
```
<ismodule 
    template= <template identifier> | <expression>
    name = "<name>"
    attribute = "<name>">
```
* **Example**
```
<!-- tag declaration -->
<ismodule template="report/report.isml" name="txtcolor" attribute="color">
<!-- tag declaration ends -->

<!-- tag usage -->
<istxtcolour color="green">

<!-- tag implementation (report.isml) -->
<isif condition="${color != null}">
   <img src="${URLUtils.webRoot() + 'images/background_'+ color+ '.gif'}">
<iselse>
   <img src="${URLUtils.webRoot() + 'images/background_default.gif'}">
</isif>
```
