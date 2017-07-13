<span data-ttu-id="ce3d1-p105">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="ce3d1-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span>| O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável |

## <span data-ttu-id="ce3d1-140">Relações</span><span class="sxs-lookup"><span data-stu-id="ce3d1-140">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="ce3d1-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce3d1-141">None</span></span>

## <span data-ttu-id="ce3d1-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce3d1-142">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="ce3d1-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce3d1-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->