# light-dom-helper-js
A light weight Document Object Model (DOM) helper

Basically this is a short cut library for coomon use dom methods.

This readme is a placeholdrr.  Please check back later for a release version of it, with examples (hope.)

## light-dom-helper creation
<script src="(path to scripts)/light-dom-helper.js"></script>
<script>const $D = build_short_dom(document)</script>


## shortdom usage
$D(node)      returns a light-dom-helper-js wrapped node, alias of build_short_dom(node)

$D(document)  returns a light-dom-helper-js wrapped document, alias of build_short_dom(document)

$D(element)   returns a light-dom-helper-js wrapped element, alias of build_short_dom(element)

$D(tagName:String, id:String, name:String, classes:String, styles:String, attrs:Obj)
                    returns the created element
$D(parent:Node, tagName:String, id:String, name:String, classes:String, styles:String, attrs:Obj)
                    returns the created element added to the parent
$D.add(parent:Node, ...(element:Node|index:number))
                    returns the element added to the parent at index or end
$D.sub(parent:Node, ...(element:Node|index:number))
                    returns the element added to the parent at index or end
$D.q(...selectors:String)
$D.q(parent:Node, selectors:String)
$D.Q(...selectors:String)
$D.Q(parent:Node, selectors:String)
$D.t(textContent:String)
                    returns the target with the textContent
$D.t(parent:Node, textContent:String)
                    returns the parent node with the textContent
$D.T(text:String)   returns a TextNode
$D.T(parent:Node, text:String)
                    returns a TextNode appended to the parent
$D(html:String)       returns a document fragment
$D(parent:Node, html:String)    returns parent with added html

$D.doc              the document
$D.head             the document head
$D.body             the document body
$D.css              the document stylesheets
$D.self             the element or document
