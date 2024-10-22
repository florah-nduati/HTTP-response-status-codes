## HTTP response status codes
# HTTP Response Status Codes

HTTP response status codes indicate the result of a specific HTTP request. They are categorized into five classes:

1. **Informational Responses (100–199)**
2. **Successful Responses (200–299)**
3. **Redirection Messages (300–399)**
4. **Client Error Responses (400–499)**
5. **Server Error Responses (500–599)**

These status codes are defined by [RFC 9110](https://datatracker.ietf.org/doc/html/rfc9110).

## Informational Responses
- **100 Continue**: The client should continue with the request or ignore the response if finished.
- **101 Switching Protocols**: The server is switching protocols as requested by the client.
- **102 Processing**: The server has received the request but is not yet complete.
- **103 Early Hints**: Used with the Link header to preload resources.

## Successful Responses
- **200 OK**: Request succeeded; response varies by method (GET, POST, etc.).
- **201 Created**: New resource has been created.
- **202 Accepted**: Request received but not yet acted upon.
- **203 Non-Authoritative Information**: Metadata differs from the origin server.
- **204 No Content**: No content to send, but headers are useful.
- **205 Reset Content**: User agent should reset the document.
- **206 Partial Content**: Partial content sent in response to a range request.
- **207 Multi-Status**: Information about multiple resources.
- **208 Already Reported**: Prevents repeated enumeration of resources.
- **226 IM Used**: Response represents the result of instance manipulations.

## Redirection Messages
- **300 Multiple Choices**: More than one response available.
- **301 Moved Permanently**: Resource has been permanently moved to a new URL.
- **302 Found**: Resource has been temporarily moved; further changes may occur.
- **303 See Other**: Resource can be found at another URI.
- **304 Not Modified**: Resource has not been modified; client can use cached version.
- **307 Temporary Redirect**: Temporary redirect with the same method used.
- **308 Permanent Redirect**: Permanent redirect; same method must be used.

## Client Error Responses
- **400 Bad Request**: Client error; malformed request.
- **401 Unauthorized**: Authentication required.
- **403 Forbidden**: Access denied to the requested resource.
- **404 Not Found**: Resource not found.
- **405 Method Not Allowed**: Method not supported by the resource.
- **409 Conflict**: Request conflicts with current server state.
- **410 Gone**: Resource permanently deleted.
- **429 Too Many Requests**: Rate limit exceeded.

## Server Error Responses
- **500 Internal Server Error**: Generic server error; unhandled situation.
- **501 Not Implemented**: Method not supported by the server.
- **502 Bad Gateway**: Invalid response from an upstream server.
- **503 Service Unavailable**: Server unable to handle the request; often due to overload.
- **504 Gateway Timeout**: Timeout when acting as a gateway.
- **511 Network Authentication Required**: Authentication needed for network access.

## Note
If you receive a response code not listed here, it may be non-standard or specific to the server's software.

