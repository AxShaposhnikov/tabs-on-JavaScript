# tabs-on-JavaScript
Algorithm

1. Get all the elements associated with tabs:
	- Tabs themselves (.info-header-tab)
	- Tab container (.info-header)
	- Blocks with content (.info-tabcontent)

2. Write a fuction that hides blocks with content. Use the 'show' and 'hide' classes in a loop where we pass through the resulting array of content blocks (tabContent[i].classList.remove ('show'), tabContent[i].classList.add ('hide') ).

3. Calling this function, starting with the element [1]. So that the element [0] remains visible.

4. Writing a function that shows hidden content. We use the 'hide' and 'show' classes. Checking if the content is hidden (tabContent[i].classList.contain('hide')) opening it.

5. Hang the event listener on the tab container. We throw the event object and use it to see which element triggered the event. If the event was triggered on an element with a tab class, i.e. on one of the tabs, we loop through the entire array of our tabs, and if our (event.target) goal matches one of the (tab[i]) tabs, we call the function to hide all content blocks [0], and call the function to open the content block, passing our tab sequence number [i] to it.
