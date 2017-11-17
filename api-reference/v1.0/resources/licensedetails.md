<span data-ttu-id="ccdb1-p104">Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ccdb1-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span>| Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura |

## <span data-ttu-id="ccdb1-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ccdb1-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="ccdb1-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccdb1-133">None</span></span>

## <span data-ttu-id="ccdb1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccdb1-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="ccdb1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccdb1-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->