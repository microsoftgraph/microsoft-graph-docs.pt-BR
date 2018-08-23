# <a name="operation-resource-type"></a><span data-ttu-id="e3c5c-101">tipo de recurso de operação</span><span class="sxs-lookup"><span data-stu-id="e3c5c-101">operation resource type</span></span>

<span data-ttu-id="e3c5c-102">O status de uma operação de longa execução.</span><span class="sxs-lookup"><span data-stu-id="e3c5c-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3c5c-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3c5c-103">JSON representation</span></span>

<span data-ttu-id="e3c5c-104">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3c5c-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="e3c5c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3c5c-105">Properties</span></span>
| <span data-ttu-id="e3c5c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c5c-106">Property</span></span>     | <span data-ttu-id="e3c5c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c5c-107">Type</span></span>   |<span data-ttu-id="e3c5c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c5c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c5c-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c5c-109">createdDateTime</span></span>| <span data-ttu-id="e3c5c-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c5c-110">DateTimeOffset</span></span> |<span data-ttu-id="e3c5c-111">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="e3c5c-111">The start time of the operation.</span></span>|
|<span data-ttu-id="e3c5c-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c5c-112">lastActionDateTime</span></span>| <span data-ttu-id="e3c5c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c5c-113">DateTimeOffset</span></span> |<span data-ttu-id="e3c5c-114">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="e3c5c-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="e3c5c-115">status</span><span class="sxs-lookup"><span data-stu-id="e3c5c-115">status</span></span>|<span data-ttu-id="e3c5c-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="e3c5c-116">operationStatus</span></span>|<span data-ttu-id="e3c5c-117">O status atual da operação: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="e3c5c-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
