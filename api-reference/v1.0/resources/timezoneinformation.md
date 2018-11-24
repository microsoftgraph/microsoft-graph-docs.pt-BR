# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="cbf75-101">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="cbf75-101">timeZoneInformation resource type</span></span>


<span data-ttu-id="cbf75-102">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cbf75-102">Represents a time zone.</span></span> <span data-ttu-id="cbf75-103">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="cbf75-103">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="cbf75-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbf75-104">Properties</span></span>
| <span data-ttu-id="cbf75-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbf75-105">Property</span></span>     | <span data-ttu-id="cbf75-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbf75-106">Type</span></span>   |<span data-ttu-id="cbf75-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbf75-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbf75-108">alias</span><span class="sxs-lookup"><span data-stu-id="cbf75-108">alias</span></span>|<span data-ttu-id="cbf75-109">string</span><span class="sxs-lookup"><span data-stu-id="cbf75-109">string</span></span>|<span data-ttu-id="cbf75-110">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cbf75-110">An identifier for the time zone.</span></span>|
|<span data-ttu-id="cbf75-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cbf75-111">displayName</span></span>|<span data-ttu-id="cbf75-112">string</span><span class="sxs-lookup"><span data-stu-id="cbf75-112">string</span></span>|<span data-ttu-id="cbf75-113">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cbf75-113">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbf75-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbf75-114">JSON representation</span></span>

<span data-ttu-id="cbf75-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbf75-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->