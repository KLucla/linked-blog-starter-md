
- Instead of GET, where user parameters are placed within the url, POST places user parameters within the HTTP request body.
- Benefits of doing this include:
	- Lack of logging
		- In the case that large files are uploaded, it would be inefficient to add all the files using GET request.
	- Less encoding requirements
		- A POST request places parameters within the body, which can be read as binary, meaning the only encoding is needed in the characters which are meant to separate parameters
	- More data can be sent
		- URL's have a maximum length, which means in certain cases they couldn't handle the amount of data needed.

- EXAMPLES OF POST
- Login Forms
- -X Post is the post flag. -d is the flag for us to put our data in.
![[Pasted image 20250421001641.png]]
- If we are authenticated, we should have received a cookie which holds our information so that next time we don't need to login when we visit the page.
- -b flag sets the cookie![[Pasted image 20250421001838.png]]
- To specify a cookie as a header, -H also works.
- In the storage tab of the DevTools, we can also view where our cookie is stored.
- You can in fact change the name and value of the cookie to a cookie with the authentication already passed, and this allows us to bypass the login screen.
- USEFUL IN ATTACKS LIKE CROSS SITE SCRIPTING


- **JSON DATA**
- In the search website, the search request is a POST request to search.php with the data in JSON code:{"search":"london"}.
- ![[Pasted image 20250421002506.png]]
- Now by specifying the content type and cookie headers, we can get a response from search.php without ever needing to login.