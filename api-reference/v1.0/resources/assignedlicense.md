# <a name="assignedlicense-resource-type"></a><span data-ttu-id="b7f25-101">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="b7f25-101">assignedLicense resource type</span></span>

<span data-ttu-id="b7f25-p101">Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="b7f25-p101">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="b7f25-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7f25-104">Properties</span></span>
| <span data-ttu-id="b7f25-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7f25-105">Property</span></span>     | <span data-ttu-id="b7f25-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7f25-106">Type</span></span>   |<span data-ttu-id="b7f25-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f25-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7f25-108">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="b7f25-108">disabledPlans</span></span>|<span data-ttu-id="b7f25-109">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="b7f25-109">Guid collection</span></span>|<span data-ttu-id="b7f25-110">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="b7f25-110">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="b7f25-111">skuId</span><span class="sxs-lookup"><span data-stu-id="b7f25-111">skuId</span></span>|<span data-ttu-id="b7f25-112">Guid</span><span class="sxs-lookup"><span data-stu-id="b7f25-112">Guid</span></span>|<span data-ttu-id="b7f25-113">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="b7f25-113">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7f25-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7f25-114">JSON representation</span></span>

<span data-ttu-id="b7f25-115">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b7f25-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
