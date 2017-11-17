# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="9d801-101">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="9d801-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="9d801-102">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9d801-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9d801-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d801-103">JSON representation</span></span>

<span data-ttu-id="9d801-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9d801-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="9d801-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d801-105">Properties</span></span>

| <span data-ttu-id="9d801-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d801-106">Property</span></span> | <span data-ttu-id="9d801-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d801-107">Type</span></span>  | <span data-ttu-id="9d801-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d801-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="9d801-109">id</span><span class="sxs-lookup"><span data-stu-id="9d801-109">id</span></span>  | <span data-ttu-id="9d801-110">string</span><span class="sxs-lookup"><span data-stu-id="9d801-110">string</span></span> | <span data-ttu-id="9d801-111">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9d801-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="9d801-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="9d801-112">persistChanges</span></span> | <span data-ttu-id="9d801-113">string</span><span class="sxs-lookup"><span data-stu-id="9d801-113">string</span></span> |  <span data-ttu-id="9d801-114">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="9d801-114">`true` for persistent session.</span></span> <span data-ttu-id="9d801-115">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="9d801-115">`false` for non-persistent session (view mode)</span></span> |

