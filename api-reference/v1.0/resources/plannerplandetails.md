# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="8b397-101">Tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8b397-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="8b397-p101">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="8b397-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="8b397-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b397-104">Methods</span></span>

| <span data-ttu-id="8b397-105">Método</span><span class="sxs-lookup"><span data-stu-id="8b397-105">Method</span></span>           | <span data-ttu-id="8b397-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b397-106">Return Type</span></span>    |<span data-ttu-id="8b397-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b397-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b397-108">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8b397-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="8b397-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8b397-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="8b397-110">Leia as propriedades e as relações do objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="8b397-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="8b397-111">Update</span><span class="sxs-lookup"><span data-stu-id="8b397-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="8b397-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8b397-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="8b397-113">Atualize o objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="8b397-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8b397-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b397-114">Properties</span></span>
| <span data-ttu-id="8b397-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b397-115">Property</span></span>     | <span data-ttu-id="8b397-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b397-116">Type</span></span>   |<span data-ttu-id="8b397-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b397-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b397-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8b397-118">categoryDescriptions</span></span>|[<span data-ttu-id="8b397-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8b397-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="8b397-120">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="8b397-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="8b397-121">id</span><span class="sxs-lookup"><span data-stu-id="8b397-121">id</span></span>|<span data-ttu-id="8b397-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b397-122">String</span></span>| <span data-ttu-id="8b397-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8b397-123">Read-only.</span></span> <span data-ttu-id="8b397-124">ID dos detalhes do plano.</span><span class="sxs-lookup"><span data-stu-id="8b397-124">ID of the plan details.</span></span> <span data-ttu-id="8b397-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8b397-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8b397-126">A [validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="8b397-126">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="8b397-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="8b397-127">sharedWith</span></span>|[<span data-ttu-id="8b397-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="8b397-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="8b397-p103">Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="8b397-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8b397-132">Relações</span><span class="sxs-lookup"><span data-stu-id="8b397-132">Relationships</span></span>
<span data-ttu-id="8b397-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b397-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b397-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b397-134">JSON representation</span></span>
<span data-ttu-id="8b397-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b397-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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