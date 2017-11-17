# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="4af8f-101">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="4af8f-101">alternativeSecurityId resource type</span></span>

<span data-ttu-id="4af8f-p101">Contém uma ID de segurança alternativa associada a um dispositivo. A propriedade **alternativeSecurityIds** da entidade [Device](device.md) é uma coleção de **alternativeSecurityId**.</span><span class="sxs-lookup"><span data-stu-id="4af8f-p101">Contains an alternative security ID associated with a device. The **alternativeSecurityIds** property of the [Device](device.md) entity is a collection of **alternativeSecurityId**.</span></span>

## <a name="properties"></a><span data-ttu-id="4af8f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4af8f-104">Properties</span></span>
| <span data-ttu-id="4af8f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4af8f-105">Property</span></span>     | <span data-ttu-id="4af8f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4af8f-106">Type</span></span>   |<span data-ttu-id="4af8f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af8f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4af8f-108">identityProvider</span><span class="sxs-lookup"><span data-stu-id="4af8f-108">identityProvider</span></span>|<span data-ttu-id="4af8f-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4af8f-109">String</span></span>|            |
|<span data-ttu-id="4af8f-110">chave</span><span class="sxs-lookup"><span data-stu-id="4af8f-110">key</span></span>|<span data-ttu-id="4af8f-111">Binário</span><span class="sxs-lookup"><span data-stu-id="4af8f-111">Binary</span></span>|            |
|<span data-ttu-id="4af8f-112">type</span><span class="sxs-lookup"><span data-stu-id="4af8f-112">type</span></span>|<span data-ttu-id="4af8f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4af8f-113">Int32</span></span>|            |

## <a name="json-representation"></a><span data-ttu-id="4af8f-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4af8f-114">JSON representation</span></span>

<span data-ttu-id="4af8f-115">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4af8f-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
