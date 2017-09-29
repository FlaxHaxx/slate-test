# user

User operations

## POST /me/user

*Information about current user*

Returns user information

> Example responses

```json
{
  "id": "string",
  "username": "string",
  "oauth2Scope": "string",
  "firstName": "string",
  "lastName": "string",
  "email": "string",
  "phone": "string"
}
```
### Responses

Status|Meaning|Description|Schema
---|---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|User information|[User](#schemauser)
401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Wrong credentials|None

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
None
</aside>





