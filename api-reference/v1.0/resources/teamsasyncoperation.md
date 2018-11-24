# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="9c132-101">tipo de recurso de teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="9c132-101">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="9c132-102">Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="9c132-102">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="9c132-103">Essas operações são muito caro concluir dentro do período de tempo de sua solicitação de origem ou de longa execução.</span><span class="sxs-lookup"><span data-stu-id="9c132-103">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="9c132-104">Quando é iniciada uma operação assíncrona, o método retornará um código de resposta 202 aceitos.</span><span class="sxs-lookup"><span data-stu-id="9c132-104">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="9c132-105">A resposta conterá também um cabeçalho de local, que contém a localização do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="9c132-105">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="9c132-106">Verificar periodicamente o status da operação, tornando uma solicitação GET para este local; Aguarde > 30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="9c132-106">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="9c132-107">Quando a solicitação for concluída com êxito, o status será "sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="9c132-107">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9c132-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c132-108">Properties</span></span>

| <span data-ttu-id="9c132-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c132-109">Property</span></span> | <span data-ttu-id="9c132-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c132-110">Type</span></span>   | <span data-ttu-id="9c132-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c132-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9c132-112">id</span><span class="sxs-lookup"><span data-stu-id="9c132-112">id</span></span>|<span data-ttu-id="9c132-113">string</span><span class="sxs-lookup"><span data-stu-id="9c132-113">string</span></span> |<span data-ttu-id="9c132-114">Id exclusiva de operação.</span><span class="sxs-lookup"><span data-stu-id="9c132-114">Unique operation id.</span></span>|
|<span data-ttu-id="9c132-115">operationType</span><span class="sxs-lookup"><span data-stu-id="9c132-115">operationType</span></span>|[<span data-ttu-id="9c132-116">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="9c132-116">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="9c132-117">Indica qual tipo de operação está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="9c132-117">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="9c132-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c132-118">createdDateTime</span></span>|<span data-ttu-id="9c132-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c132-119">DateTimeOffset</span></span> |<span data-ttu-id="9c132-120">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="9c132-120">Time when the operation was created.</span></span>|
|<span data-ttu-id="9c132-121">status</span><span class="sxs-lookup"><span data-stu-id="9c132-121">status</span></span>|[<span data-ttu-id="9c132-122">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="9c132-122">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="9c132-123">Status de operação.</span><span class="sxs-lookup"><span data-stu-id="9c132-123">Operation status.</span></span>|
|<span data-ttu-id="9c132-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9c132-124">lastActionDateTime</span></span>|<span data-ttu-id="9c132-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c132-125">DateTimeOffset</span></span> |<span data-ttu-id="9c132-126">Hora de quando a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9c132-126">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="9c132-127">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="9c132-127">attemptsCount</span></span>|<span data-ttu-id="9c132-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9c132-128">Int32</span></span>|<span data-ttu-id="9c132-129">Número de vezes que a operação foi tentada antes de serem marcadas com êxito ou falha.</span><span class="sxs-lookup"><span data-stu-id="9c132-129">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="9c132-130">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="9c132-130">targetResourceId</span></span>|<span data-ttu-id="9c132-131">GUID</span><span class="sxs-lookup"><span data-stu-id="9c132-131">guid</span></span> |<span data-ttu-id="9c132-132">A identificação do objeto que tenha criado ou modificado como resultado dessa operação assíncrona, geralmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9c132-132">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="9c132-133">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="9c132-133">targetResourceLocation</span></span>|<span data-ttu-id="9c132-134">string</span><span class="sxs-lookup"><span data-stu-id="9c132-134">string</span></span>|<span data-ttu-id="9c132-135">O local do objeto que tenha criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="9c132-135">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="9c132-136">Essa URL deve ser tratado como um valor opaco e não analisado em caminhos de seus componentes.</span><span class="sxs-lookup"><span data-stu-id="9c132-136">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="9c132-137">erro</span><span class="sxs-lookup"><span data-stu-id="9c132-137">error</span></span>|[<span data-ttu-id="9c132-138">operationError</span><span class="sxs-lookup"><span data-stu-id="9c132-138">operationError</span></span>](operationerror.md)|<span data-ttu-id="9c132-139">Qualquer erro que faz com que a operação assíncrona falhe.</span><span class="sxs-lookup"><span data-stu-id="9c132-139">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c132-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c132-140">JSON representation</span></span>

<span data-ttu-id="9c132-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c132-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
