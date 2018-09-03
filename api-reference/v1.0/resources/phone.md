# <a name="phone-resource-type"></a><span data-ttu-id="dbdd6-101">Tipo de recurso phone</span><span class="sxs-lookup"><span data-stu-id="dbdd6-101">phone resource type</span></span>

<span data-ttu-id="dbdd6-102">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="dbdd6-102">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="dbdd6-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbdd6-103">Properties</span></span>
| <span data-ttu-id="dbdd6-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbdd6-104">Property</span></span>     | <span data-ttu-id="dbdd6-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbdd6-105">Type</span></span>   |<span data-ttu-id="dbdd6-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbdd6-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbdd6-107">number</span><span class="sxs-lookup"><span data-stu-id="dbdd6-107">number</span></span>|<span data-ttu-id="dbdd6-108">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbdd6-108">string</span></span>|<span data-ttu-id="dbdd6-109">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="dbdd6-109">The phone number.</span></span>|
|<span data-ttu-id="dbdd6-110">type</span><span class="sxs-lookup"><span data-stu-id="dbdd6-110">type</span></span>|<span data-ttu-id="dbdd6-111">phoneType</span><span class="sxs-lookup"><span data-stu-id="dbdd6-111">phoneType values</span></span>|<span data-ttu-id="dbdd6-112">O tipo de número de telefone.</span><span class="sxs-lookup"><span data-stu-id="dbdd6-112">The type of phone number.</span></span> <span data-ttu-id="dbdd6-113">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="dbdd6-113">The possible values are `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`, , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbdd6-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbdd6-114">JSON representation</span></span>

<span data-ttu-id="dbdd6-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbdd6-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
