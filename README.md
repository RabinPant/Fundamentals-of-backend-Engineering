# Fundamentals-of-backend-Engineering

# Design Patterns:

## Request-Response:

- This is one of the most simplest and elegant design pattern. Here client simply sends the request with payload and server response with the body.
- Client sends request, server parses the request, server process the request, server sends the response and client parses the response.

- where it can be use:
    - HTTP, RTC, graphQL, REST etc.
  <br>
  ### Building an upload image service with request and response:
 - There are two different ways to implement this.
 - first way is to simply send large request with image but if we fail in this operation there is no resuming of this operation.
 - The second approach which is also the best approach is to chunk the image and send reqeust per chunk. This operaion is resumable.

   ### where request-reponse doesn't work?
   - Notification service
   - chatting application

     <br>
     Example with CURL:<br>
     curl -v --trace output.txt http://google.com <br>
     This will provide you with the proper request - response and it structure under HTTP.
