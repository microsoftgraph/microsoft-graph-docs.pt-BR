<span data-ttu-id="7a527-p142">Os threads de conversas do grupo. Anulável.</span><span class="sxs-lookup"><span data-stu-id="7a527-p142">The group's conversation threads. Nullable.</span></span>| Os threads de conversas do grupo. Anulável.|


## <a name="json-representation"></a><span data-ttu-id="7a527-436">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a527-436">JSON representation</span></span>

<span data-ttu-id="7a527-437">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a527-437">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": ["string"],
  "securityEnabled": true,
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a><span data-ttu-id="7a527-438">Veja também</span><span class="sxs-lookup"><span data-stu-id="7a527-438">See also</span></span>

- [<span data-ttu-id="7a527-439">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7a527-439">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7a527-440">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="7a527-440">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="7a527-441">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="7a527-441">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
