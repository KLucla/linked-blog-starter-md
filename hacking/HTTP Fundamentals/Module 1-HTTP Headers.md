- Headers pass information back and forth between the client and the server.
- Some headers are unique to a request/response and some are shared
- Headers can have one or multiple values, appended after the header name and separated by a colon.

- **GENERAL HEADERS**
![[Pasted image 20250419225049.png]]
- **ENTITY HEADERS**
![[Pasted image 20250419225133.png]]
- **REQUEST HEADERS**
![[Pasted image 20250419225205.png]]
- Cookies are both client side and server side, while authorization tokens are stored only on the client side.
- A complete list of request headers and their usage can be found [here](https://tools.ietf.org/html/rfc7231#section-5).
- **RESPONSE HEADERS**
![[Pasted image 20250419225341.png]]

- **SECURITY HEADERS**
![[Pasted image 20250419225410.png]]



- cURL
- -I is used to view the response headers
- e.g. KLhcks@htb[/htb]$ curl -I https://www.inlanefreight.com
- -H can be used to set the request headers,
	- -A can be used to set the user agent


- **BROWSER DEVTOOLS**
- 