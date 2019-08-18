bento orange.small{}
-select all <orange> elements with a class of small who are children of <bento> elements

orange.small{}
-select all <orange> elements with a class of small

#fancy pickle{}
-select all <pickle> elements who are children of elements with an id of #fancy

*{}
-selects everyfreakingthing

plate + apple{}
-selects all <apple> elements that directly follow under <plate> elements that are siblings.

bento ~ pickle
-selects all <pickle> elements following <bento> elements that are siblings.

plate > apple
-selects all <apple> elements that are direct children of <plate> elements.

So, 
<plate>
  <apple>
</plate>
but not
<plate>
  <bananna>
  <apple>
</plate>

plate :first-child
-selects only the first child element of the <plate> element

plate :only-child
-selects only elements that are children of <plate> elements and the only element inside the <plate> element

pickle.small,#fancy last:child
-selects only the element <pickle> with a class of .small, and the last child of any element with the the #fancy id


