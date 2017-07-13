<span data-ttu-id="ea7a5-p105">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="ea7a5-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span>| O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável |
|<span data-ttu-id="ea7a5-149">weight</span><span class="sxs-lookup"><span data-stu-id="ea7a5-149">weight</span></span>|<span data-ttu-id="ea7a5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ea7a5-150">Int32</span></span>| <span data-ttu-id="ea7a5-151">O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ea7a5-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <span data-ttu-id="ea7a5-152">Relações</span><span class="sxs-lookup"><span data-stu-id="ea7a5-152">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="ea7a5-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea7a5-153">None</span></span>


## <span data-ttu-id="ea7a5-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea7a5-154">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="ea7a5-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea7a5-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->