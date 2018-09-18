# <a name="security-resource-type"></a><span data-ttu-id="3ddd8-101">tipo de recurso Security</span><span class="sxs-lookup"><span data-stu-id="3ddd8-101">security resource type</span></span>

<span data-ttu-id="3ddd8-102">O recurso Security é o ponto de entrada para o modelo de objeto de segurança.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-102">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="3ddd8-103">Ele retorna um recurso security singleton.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-103">It returns a singleton security resource.</span></span> <span data-ttu-id="3ddd8-104">Não contém nenhuma propriedade utilizável.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-104">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3ddd8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3ddd8-105">Methods</span></span>

| <span data-ttu-id="3ddd8-106">Método</span><span class="sxs-lookup"><span data-stu-id="3ddd8-106">Method</span></span>       | <span data-ttu-id="3ddd8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3ddd8-107">Return Type</span></span> | <span data-ttu-id="3ddd8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ddd8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ddd8-109">List alertas</span><span class="sxs-lookup"><span data-stu-id="3ddd8-109">List alerts</span></span>](../api/alert_list.md) | <span data-ttu-id="3ddd8-110">coleção [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="3ddd8-110">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ddd8-111">Obtém uma coleção de objetos alert.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-111">Get a licenseDetails object collection.</span></span> |
| [<span data-ttu-id="3ddd8-112">get alerts</span><span class="sxs-lookup"><span data-stu-id="3ddd8-112">get alerts</span></span>](../api/alert_get.md) | <span data-ttu-id="3ddd8-113">coleção [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="3ddd8-113">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ddd8-114">Obtém um objeto alert.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-114">Get a alert object.</span></span> |
| [<span data-ttu-id="3ddd8-115">Update alerts</span><span class="sxs-lookup"><span data-stu-id="3ddd8-115">Update alerts</span></span>](../api/alert_update.md) | <span data-ttu-id="3ddd8-116">coleção [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="3ddd8-116">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ddd8-117">Obtém um objeto alert.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-117">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ddd8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ddd8-118">Properties</span></span>
<span data-ttu-id="3ddd8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ddd8-119">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3ddd8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3ddd8-120">Relationships</span></span>
| <span data-ttu-id="3ddd8-121">Relação</span><span class="sxs-lookup"><span data-stu-id="3ddd8-121">Relationship</span></span> | <span data-ttu-id="3ddd8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ddd8-122">Type</span></span>        | <span data-ttu-id="3ddd8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ddd8-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ddd8-124">alerts</span><span class="sxs-lookup"><span data-stu-id="3ddd8-124">alerts</span></span>|<span data-ttu-id="3ddd8-125">coleção [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="3ddd8-125">[alert](alert.md) collection</span></span>| <span data-ttu-id="3ddd8-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-p102">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3ddd8-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ddd8-128">JSON representation</span></span>
<span data-ttu-id="3ddd8-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="3ddd8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ddd8-130">Example</span></span>

<span data-ttu-id="3ddd8-131">O recurso **security** está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="3ddd8-131">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
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
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->