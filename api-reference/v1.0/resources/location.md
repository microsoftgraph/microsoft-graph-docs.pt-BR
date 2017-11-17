# <a name="location-resource-type"></a><span data-ttu-id="842c5-101">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="842c5-101">Location resource type</span></span>

<span data-ttu-id="842c5-102">Representa informações de localização para um evento.</span><span class="sxs-lookup"><span data-stu-id="842c5-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="842c5-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="842c5-103">Properties</span></span>
| <span data-ttu-id="842c5-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="842c5-104">Property</span></span>  | <span data-ttu-id="842c5-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="842c5-105">Type</span></span>   | <span data-ttu-id="842c5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="842c5-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="842c5-107">address</span><span class="sxs-lookup"><span data-stu-id="842c5-107">address</span></span> | [<span data-ttu-id="842c5-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="842c5-108">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="842c5-109">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="842c5-109">The street address of the location.</span></span> |
| <span data-ttu-id="842c5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="842c5-110">displayName</span></span>  | <span data-ttu-id="842c5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c5-111">String</span></span> | <span data-ttu-id="842c5-112">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="842c5-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="842c5-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="842c5-113">locationEmailAddress</span></span> | <span data-ttu-id="842c5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c5-114">String</span></span> | <span data-ttu-id="842c5-115">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="842c5-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="842c5-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="842c5-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a><span data-ttu-id="842c5-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="842c5-117">Remarks</span></span>

<span data-ttu-id="842c5-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="842c5-118">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->