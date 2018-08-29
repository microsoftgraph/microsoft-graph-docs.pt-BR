# <a name="filtercriteria-resource-type"></a><span data-ttu-id="863b8-101">Tipo de recurso FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="863b8-101">FilterCriteria resource type</span></span>

<span data-ttu-id="863b8-102">Representa os critérios de filtragem aplicados a uma coluna.</span><span class="sxs-lookup"><span data-stu-id="863b8-102">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="863b8-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="863b8-103">JSON representation</span></span>

<span data-ttu-id="863b8-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="863b8-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "icon": {"@odata.type": "microsoft.graph.workbookIcon"},
  "values": {"@odata.type": "microsoft.graph.Json"}
}

```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'color' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion1' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion2' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'dynamicCriteria' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'filterOn' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'icon' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'values' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table."
  ]
} -->