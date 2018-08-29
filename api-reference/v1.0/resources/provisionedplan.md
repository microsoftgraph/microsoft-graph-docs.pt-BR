# <a name="provisionedplan-resource-type"></a><span data-ttu-id="d6f94-101">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="d6f94-101">provisionedPlan resource type</span></span>

<span data-ttu-id="d6f94-102">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="d6f94-102">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="d6f94-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6f94-103">Properties</span></span>
| <span data-ttu-id="d6f94-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6f94-104">Property</span></span>     | <span data-ttu-id="d6f94-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6f94-105">Type</span></span>   |<span data-ttu-id="d6f94-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6f94-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6f94-107">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d6f94-107">capabilityStatus</span></span>|<span data-ttu-id="d6f94-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6f94-108">String</span></span>|<span data-ttu-id="d6f94-109">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="d6f94-109">For example, “Enabled”.</span></span>|
|<span data-ttu-id="d6f94-110">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="d6f94-110">provisioningStatus</span></span>|<span data-ttu-id="d6f94-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6f94-111">String</span></span>|<span data-ttu-id="d6f94-112">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="d6f94-112">For example, “Success”.</span></span>|
|<span data-ttu-id="d6f94-113">service</span><span class="sxs-lookup"><span data-stu-id="d6f94-113">service</span></span>|<span data-ttu-id="d6f94-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6f94-114">String</span></span>|<span data-ttu-id="d6f94-115">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="d6f94-115">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6f94-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6f94-116">JSON representation</span></span>

<span data-ttu-id="d6f94-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d6f94-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->