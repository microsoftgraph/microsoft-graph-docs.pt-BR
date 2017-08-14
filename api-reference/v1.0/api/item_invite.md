<span data-ttu-id="27d06-p102">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="27d06-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>                                          | Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres. |
| <span data-ttu-id="27d06-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="27d06-122">requireSignIn</span></span>    | <span data-ttu-id="27d06-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="27d06-123">Boolean</span></span>                                         | <span data-ttu-id="27d06-124">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="27d06-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="27d06-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="27d06-125">sendInvitation</span></span>   | <span data-ttu-id="27d06-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="27d06-126">Boolean</span></span>                                         | <span data-ttu-id="27d06-127">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="27d06-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="27d06-128">funções</span><span class="sxs-lookup"><span data-stu-id="27d06-128">roles</span></span>            | <span data-ttu-id="27d06-129">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="27d06-129">Collection(String)</span></span>                              | <span data-ttu-id="27d06-130">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="27d06-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="27d06-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d06-131">Response</span></span>

<span data-ttu-id="27d06-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d06-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27d06-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27d06-133">Example</span></span>
<span data-ttu-id="27d06-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="27d06-134">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="27d06-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d06-135">Request</span></span>
<span data-ttu-id="27d06-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d06-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="27d06-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d06-137">Response</span></span>
<span data-ttu-id="27d06-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d06-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="27d06-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="27d06-139">Remarks</span></span>

* <span data-ttu-id="27d06-140">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="27d06-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="27d06-141">Para obter uma lista das funções disponíveis, confira [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="27d06-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
