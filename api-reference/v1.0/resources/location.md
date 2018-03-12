# <a name="location-resource-type"></a><span data-ttu-id="acbda-101">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="acbda-101">Location resource type</span></span>

<span data-ttu-id="acbda-102">Representa informações de localização para um evento.</span><span class="sxs-lookup"><span data-stu-id="acbda-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="acbda-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acbda-103">Properties</span></span>
| <span data-ttu-id="acbda-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acbda-104">Property</span></span>  | <span data-ttu-id="acbda-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="acbda-105">Type</span></span>   | <span data-ttu-id="acbda-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="acbda-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="acbda-107">address</span><span class="sxs-lookup"><span data-stu-id="acbda-107">address</span></span> | [<span data-ttu-id="acbda-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="acbda-108">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="acbda-109">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="acbda-109">The street address of the location.</span></span> |
| <span data-ttu-id="acbda-110">displayName</span><span class="sxs-lookup"><span data-stu-id="acbda-110">displayName</span></span>  | <span data-ttu-id="acbda-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acbda-111">String</span></span> | <span data-ttu-id="acbda-112">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="acbda-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="acbda-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="acbda-113">locationEmailAddress</span></span> | <span data-ttu-id="acbda-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acbda-114">String</span></span> | <span data-ttu-id="acbda-115">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="acbda-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="acbda-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acbda-116">JSON representation</span></span>

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

## <a name="remarks"></a><span data-ttu-id="acbda-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="acbda-117">Remarks</span></span>

<span data-ttu-id="acbda-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="acbda-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
