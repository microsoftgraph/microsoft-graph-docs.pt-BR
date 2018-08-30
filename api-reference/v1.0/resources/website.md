# <a name="website-resource-type"></a><span data-ttu-id="81459-101">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="81459-101">website resource type</span></span>

<span data-ttu-id="81459-102">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="81459-102">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="81459-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81459-103">Properties</span></span>
| <span data-ttu-id="81459-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81459-104">Property</span></span>     | <span data-ttu-id="81459-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="81459-105">Type</span></span>   |<span data-ttu-id="81459-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="81459-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81459-107">type</span><span class="sxs-lookup"><span data-stu-id="81459-107">type</span></span>|<span data-ttu-id="81459-108">websiteType</span><span class="sxs-lookup"><span data-stu-id="81459-108">WebsiteType</span></span>| <span data-ttu-id="81459-109">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="81459-109">The possible values are `other`, `home`, `work`, `blog`, `profile`, , , , , , , or .</span></span>|
|<span data-ttu-id="81459-110">address</span><span class="sxs-lookup"><span data-stu-id="81459-110">address</span></span>|<span data-ttu-id="81459-111">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="81459-111">string</span></span>|<span data-ttu-id="81459-112">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="81459-112">The URL of the website.</span></span>|
|<span data-ttu-id="81459-113">displayName</span><span class="sxs-lookup"><span data-stu-id="81459-113">displayName</span></span>|<span data-ttu-id="81459-114">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="81459-114">string</span></span>|<span data-ttu-id="81459-115">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="81459-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81459-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81459-116">JSON representation</span></span>

<span data-ttu-id="81459-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81459-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
