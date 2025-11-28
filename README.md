# JAVASCRIPT : Why-direct-DOM-manipulation-is-preferred-over-innerHTML-for-tables-in-Javascript
Populating a table using direct DOM manipulation methods is generally preferred over innerHTML for security, performance, and maintainability, especially when dealing with dynamic or user-generated content
#Security (XSS Prevention): 
innerHTML allows the injection of raw HTML, including malicious scripts. If you're populating a table with data from an untrusted source, using innerHTML can expose your application to Cross-Site Scripting (XSS) attacks. Direct DOM manipulation, by creating elements and setting their textContent, prevents script execution.
#	Performance (for complex structures/large datasets): 
While innerHTML can be faster for very simple, one-time insertions, for building complex structures like tables with many rows and cells, especially when dealing with large datasets, creating and appending individual DOM nodes can be more efficient. innerHTML involves parsing a string into DOM elements, which can be a performance bottleneck.
