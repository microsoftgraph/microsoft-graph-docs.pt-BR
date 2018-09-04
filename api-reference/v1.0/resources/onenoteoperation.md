# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="d157b-101">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="d157b-101">onenoteOperation resource type</span></span>

<span data-ttu-id="d157b-102">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d157b-102">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d157b-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d157b-103">JSON representation</span></span>

<span data-ttu-id="d157b-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d157b-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d157b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d157b-105">Properties</span></span>
| <span data-ttu-id="d157b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d157b-106">Property</span></span>     | <span data-ttu-id="d157b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d157b-107">Type</span></span>   |<span data-ttu-id="d157b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d157b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d157b-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d157b-109">createdDateTime</span></span>| <span data-ttu-id="d157b-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d157b-110">DateTimeOffset</span></span> |<span data-ttu-id="d157b-111">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="d157b-111">The start time of the operation.</span></span>|
|<span data-ttu-id="d157b-112">erro</span><span class="sxs-lookup"><span data-stu-id="d157b-112">error</span></span>|[<span data-ttu-id="d157b-113">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="d157b-113">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="d157b-114">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="d157b-114">The error returned by the operation.</span></span>|
|<span data-ttu-id="d157b-115">id</span><span class="sxs-lookup"><span data-stu-id="d157b-115">id</span></span>|<span data-ttu-id="d157b-116">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d157b-116">string</span></span>|<span data-ttu-id="d157b-117">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d157b-117">The operation id. Read-only.</span></span>|
|<span data-ttu-id="d157b-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d157b-118">lastActionDateTime</span></span>| <span data-ttu-id="d157b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d157b-119">DateTimeOffset</span></span> |<span data-ttu-id="d157b-120">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="d157b-120">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="d157b-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="d157b-121">resourceId</span></span>|<span data-ttu-id="d157b-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d157b-122">string</span></span>|<span data-ttu-id="d157b-123">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="d157b-123">The resource id.</span></span>|
|<span data-ttu-id="d157b-124">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="d157b-124">resourceLocation</span></span>|<span data-ttu-id="d157b-125">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d157b-125">string</span></span>|<span data-ttu-id="d157b-p101">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="d157b-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="d157b-128">status</span><span class="sxs-lookup"><span data-stu-id="d157b-128">status</span></span>|<span data-ttu-id="d157b-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d157b-129">string</span></span>|<span data-ttu-id="d157b-130">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="d157b-130">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="d157b-131">percentComplete</span><span class="sxs-lookup"><span data-stu-id="d157b-131">percentComplete</span></span>|<span data-ttu-id="d157b-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d157b-132">string</span></span>|<span data-ttu-id="d157b-133">A porcentagem concluída da operação se a operação ainda estiver com um status`running`</span><span class="sxs-lookup"><span data-stu-id="d157b-133">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="d157b-134">Relações</span><span class="sxs-lookup"><span data-stu-id="d157b-134">Relationships</span></span>
<span data-ttu-id="d157b-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d157b-135">None</span></span>


## <a name="methods"></a><span data-ttu-id="d157b-136">Métodos</span><span class="sxs-lookup"><span data-stu-id="d157b-136">Methods</span></span>

| <span data-ttu-id="d157b-137">Método</span><span class="sxs-lookup"><span data-stu-id="d157b-137">Method</span></span>           | <span data-ttu-id="d157b-138">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d157b-138">Return Type</span></span>    |<span data-ttu-id="d157b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d157b-139">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d157b-140">Get operation</span><span class="sxs-lookup"><span data-stu-id="d157b-140">Get operation</span></span>](../api/onenoteoperation_get.md) | [<span data-ttu-id="d157b-141">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="d157b-141">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="d157b-142">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="d157b-142">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
