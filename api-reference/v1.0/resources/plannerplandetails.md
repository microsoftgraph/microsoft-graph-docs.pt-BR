# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="a8b63-101">Tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8b63-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="a8b63-p101">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="a8b63-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="a8b63-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="a8b63-104">Methods</span></span>

| <span data-ttu-id="a8b63-105">Método</span><span class="sxs-lookup"><span data-stu-id="a8b63-105">Method</span></span>           | <span data-ttu-id="a8b63-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a8b63-106">Return Type</span></span>    |<span data-ttu-id="a8b63-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b63-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8b63-108">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8b63-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="a8b63-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8b63-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="a8b63-110">Leia as propriedades e as relações do objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="a8b63-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="a8b63-111">Update</span><span class="sxs-lookup"><span data-stu-id="a8b63-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="a8b63-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8b63-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="a8b63-113">Atualize o objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="a8b63-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a8b63-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b63-114">Properties</span></span>
| <span data-ttu-id="a8b63-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b63-115">Property</span></span>     | <span data-ttu-id="a8b63-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b63-116">Type</span></span>   |<span data-ttu-id="a8b63-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b63-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8b63-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a8b63-118">categoryDescriptions</span></span>|[<span data-ttu-id="a8b63-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a8b63-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="a8b63-120">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="a8b63-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="a8b63-121">id</span><span class="sxs-lookup"><span data-stu-id="a8b63-121">id</span></span>|<span data-ttu-id="a8b63-122">String</span><span class="sxs-lookup"><span data-stu-id="a8b63-122">String</span></span>| <span data-ttu-id="a8b63-p102">Somente leitura. ID dos detalhes dos planos. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="a8b63-p102">Read-only. ID of the plan details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a8b63-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="a8b63-127">sharedWith</span></span>|[<span data-ttu-id="a8b63-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a8b63-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="a8b63-p103">Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="a8b63-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a8b63-132">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b63-132">Relationships</span></span>
<span data-ttu-id="a8b63-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b63-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a8b63-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b63-134">JSON representation</span></span>
<span data-ttu-id="a8b63-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8b63-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->