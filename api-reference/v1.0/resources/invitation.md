<span data-ttu-id="468ba-p108">O usuário criado como parte da criação do convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="468ba-p108">The user created as part of the invitation creation. Read-Only</span></span>|O usuário criado como parte da criação do convite. Somente leitura|

## <span data-ttu-id="468ba-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="468ba-165">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="468ba-166">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="468ba-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
