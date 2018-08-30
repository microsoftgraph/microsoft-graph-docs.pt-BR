# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="bd5dc-101">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="bd5dc-101">locationConstraintItem resource type</span></span>

<span data-ttu-id="bd5dc-102">As condições indicadas por um cliente para a localização de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="bd5dc-102">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="bd5dc-103">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="bd5dc-103">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd5dc-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd5dc-104">JSON representation</span></span>

<span data-ttu-id="bd5dc-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bd5dc-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bd5dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd5dc-106">Properties</span></span>
| <span data-ttu-id="bd5dc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd5dc-107">Property</span></span>     | <span data-ttu-id="bd5dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd5dc-108">Type</span></span>   |<span data-ttu-id="bd5dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd5dc-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bd5dc-110">address</span><span class="sxs-lookup"><span data-stu-id="bd5dc-110">address</span></span> | [<span data-ttu-id="bd5dc-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="bd5dc-111">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="bd5dc-112">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="bd5dc-112">The street address of the location.</span></span> |
| <span data-ttu-id="bd5dc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bd5dc-113">displayName</span></span>  | <span data-ttu-id="bd5dc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd5dc-114">String</span></span> | <span data-ttu-id="bd5dc-115">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="bd5dc-115">The name associated with the location.</span></span>                       |
| <span data-ttu-id="bd5dc-116">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bd5dc-116">locationEmailAddress</span></span> | <span data-ttu-id="bd5dc-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd5dc-117">String</span></span> | <span data-ttu-id="bd5dc-118">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="bd5dc-118">Optional email address of the location.</span></span> |
| <span data-ttu-id="bd5dc-119">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="bd5dc-119">resolveAvailability</span></span> | <span data-ttu-id="bd5dc-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="bd5dc-120">Boolean</span></span> | <span data-ttu-id="bd5dc-p101">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user_findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="bd5dc-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user_findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->