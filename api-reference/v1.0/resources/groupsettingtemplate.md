<span data-ttu-id="c8f16-p102">O identificador exclusivo do modelo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8f16-p102">Unique identifier for the subscription. Read-only.</span></span>| O identificador exclusivo do modelo. Somente leitura.|
|<span data-ttu-id="c8f16-131">values</span><span class="sxs-lookup"><span data-stu-id="c8f16-131">values</span></span>|<span data-ttu-id="c8f16-132">Conjunto [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="c8f16-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="c8f16-133">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.</span><span class="sxs-lookup"><span data-stu-id="c8f16-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8f16-134">Relações</span><span class="sxs-lookup"><span data-stu-id="c8f16-134">Relationships</span></span>

<span data-ttu-id="c8f16-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8f16-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c8f16-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8f16-136">JSON representation</span></span>

<span data-ttu-id="c8f16-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8f16-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->