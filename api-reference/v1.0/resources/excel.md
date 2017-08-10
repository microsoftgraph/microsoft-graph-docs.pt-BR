<span data-ttu-id="afa6f-p120">Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.</span><span class="sxs-lookup"><span data-stu-id="afa6f-p120">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span> 

Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.
 
<span data-ttu-id="afa6f-277">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="afa6f-277">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

