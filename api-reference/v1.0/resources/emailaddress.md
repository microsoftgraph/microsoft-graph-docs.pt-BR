# <a name="emailaddress-resource-type"></a><span data-ttu-id="d01aa-101">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="d01aa-101">emailAddress resource type</span></span>

<span data-ttu-id="d01aa-102">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="d01aa-102">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="d01aa-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d01aa-103">Properties</span></span>
| <span data-ttu-id="d01aa-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d01aa-104">Property</span></span>     | <span data-ttu-id="d01aa-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="d01aa-105">Type</span></span>   |<span data-ttu-id="d01aa-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d01aa-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d01aa-107">address</span><span class="sxs-lookup"><span data-stu-id="d01aa-107">address</span></span>|<span data-ttu-id="d01aa-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d01aa-108">String</span></span>|<span data-ttu-id="d01aa-109">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="d01aa-109">The email address of the person or entity.</span></span>|
|<span data-ttu-id="d01aa-110">name</span><span class="sxs-lookup"><span data-stu-id="d01aa-110">name</span></span>|<span data-ttu-id="d01aa-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d01aa-111">String</span></span>|<span data-ttu-id="d01aa-112">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="d01aa-112">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d01aa-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d01aa-113">JSON representation</span></span>

<span data-ttu-id="d01aa-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d01aa-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
