# <a name="sizerange-resource-type"></a><span data-ttu-id="09684-101">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="09684-101">sizeRange resource type</span></span>


<span data-ttu-id="09684-102">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="09684-102">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="09684-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09684-103">Properties</span></span>
| <span data-ttu-id="09684-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09684-104">Property</span></span>     | <span data-ttu-id="09684-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="09684-105">Type</span></span>   |<span data-ttu-id="09684-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="09684-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09684-107">maximumSize</span><span class="sxs-lookup"><span data-stu-id="09684-107">maximumSize</span></span> | <span data-ttu-id="09684-108">Int32</span><span class="sxs-lookup"><span data-stu-id="09684-108">Int32</span></span> | <span data-ttu-id="09684-109">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="09684-109">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="09684-110">minimumSize</span><span class="sxs-lookup"><span data-stu-id="09684-110">minimumSize</span></span> | <span data-ttu-id="09684-111">Int32</span><span class="sxs-lookup"><span data-stu-id="09684-111">Int32</span></span> | <span data-ttu-id="09684-112">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="09684-112">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="09684-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09684-113">JSON representation</span></span>
<span data-ttu-id="09684-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09684-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->