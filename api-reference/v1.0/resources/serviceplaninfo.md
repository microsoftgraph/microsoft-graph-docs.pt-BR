<span data-ttu-id="52e6f-p103">O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="52e6f-p103">The object the service plan can be assigned to. Possible values:</span></span>|O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:<br/><span data-ttu-id="52e6f-127">"Usuário" – o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="52e6f-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="52e6f-128">"Empresa" – o plano de serviço pode ser atribuído a todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="52e6f-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52e6f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52e6f-129">JSON representation</span></span>

<span data-ttu-id="52e6f-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="52e6f-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
