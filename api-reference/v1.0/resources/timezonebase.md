# <a name="timezonebase-resource-type"></a><span data-ttu-id="e77f8-101">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="e77f8-101">timeZoneBase resource type</span></span>

<span data-ttu-id="e77f8-102">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e77f8-102">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="e77f8-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e77f8-103">Properties</span></span>
| <span data-ttu-id="e77f8-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e77f8-104">Property</span></span>     | <span data-ttu-id="e77f8-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="e77f8-105">Type</span></span>   |<span data-ttu-id="e77f8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e77f8-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e77f8-107">name</span><span class="sxs-lookup"><span data-stu-id="e77f8-107">name</span></span> | <span data-ttu-id="e77f8-108">string</span><span class="sxs-lookup"><span data-stu-id="e77f8-108">string</span></span> | <span data-ttu-id="e77f8-109">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e77f8-109">The name of a time zone.</span></span> <span data-ttu-id="e77f8-110">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="e77f8-110">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e77f8-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e77f8-111">JSON representation</span></span>

<span data-ttu-id="e77f8-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e77f8-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->