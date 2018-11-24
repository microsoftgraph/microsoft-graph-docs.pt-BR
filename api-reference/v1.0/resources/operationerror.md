# <a name="operationerror-resource-type"></a><span data-ttu-id="6e581-101">tipo de recurso de operationError</span><span class="sxs-lookup"><span data-stu-id="6e581-101">operationError resource type</span></span>



<span data-ttu-id="6e581-102">Descreve os erros em [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6e581-102">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="6e581-103">Propriedades de operationError</span><span class="sxs-lookup"><span data-stu-id="6e581-103">operationError Properties</span></span>
| <span data-ttu-id="6e581-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e581-104">Property</span></span>     | <span data-ttu-id="6e581-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e581-105">Type</span></span>   |<span data-ttu-id="6e581-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e581-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e581-107">código</span><span class="sxs-lookup"><span data-stu-id="6e581-107">code</span></span>|<span data-ttu-id="6e581-108">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="6e581-108">string (readonly)</span></span>|<span data-ttu-id="6e581-109">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="6e581-109">Operation error code.</span></span>|
|<span data-ttu-id="6e581-110">message</span><span class="sxs-lookup"><span data-stu-id="6e581-110">message</span></span>|<span data-ttu-id="6e581-111">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="6e581-111">string (readonly)</span></span>|<span data-ttu-id="6e581-112">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="6e581-112">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e581-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e581-113">JSON representation</span></span>

<span data-ttu-id="6e581-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e581-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
