# <a name="planner-resource-type"></a><span data-ttu-id="8f637-101">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="8f637-101">planner resource type</span></span>

<span data-ttu-id="8f637-p101">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="8f637-p101">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="8f637-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f637-105">Methods</span></span>

| <span data-ttu-id="8f637-106">Método</span><span class="sxs-lookup"><span data-stu-id="8f637-106">Method</span></span>           | <span data-ttu-id="8f637-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f637-107">Return Type</span></span>    |<span data-ttu-id="8f637-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f637-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f637-109">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8f637-109">Create plannerBucket</span></span>](../api/planner_post_buckets.md) |[<span data-ttu-id="8f637-110">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8f637-110">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="8f637-111">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="8f637-111">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="8f637-112">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="8f637-112">Create plannerPlan</span></span>](../api/planner_post_plans.md) |[<span data-ttu-id="8f637-113">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="8f637-113">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="8f637-114">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="8f637-114">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="8f637-115">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="8f637-115">Create plannerTask</span></span>](../api/planner_post_tasks.md) |[<span data-ttu-id="8f637-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="8f637-116">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="8f637-117">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="8f637-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f637-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8f637-118">Relationships</span></span>
| <span data-ttu-id="8f637-119">Relação</span><span class="sxs-lookup"><span data-stu-id="8f637-119">Relationship</span></span> | <span data-ttu-id="8f637-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f637-120">Type</span></span>   |<span data-ttu-id="8f637-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f637-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f637-122">buckets</span><span class="sxs-lookup"><span data-stu-id="8f637-122">buckets</span></span>|<span data-ttu-id="8f637-123">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="8f637-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="8f637-p102">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="8f637-p102">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="8f637-127">plans</span><span class="sxs-lookup"><span data-stu-id="8f637-127">plans</span></span>|<span data-ttu-id="8f637-128">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8f637-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8f637-p103">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="8f637-p103">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="8f637-132">tarefas</span><span class="sxs-lookup"><span data-stu-id="8f637-132">tasks</span></span>|<span data-ttu-id="8f637-133">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="8f637-133">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="8f637-p104">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="8f637-p104">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f637-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f637-137">JSON representation</span></span>
<span data-ttu-id="8f637-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f637-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="8f637-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f637-139">Example</span></span>

<span data-ttu-id="8f637-140">O recurso de **planner** estará disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="8f637-140">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->