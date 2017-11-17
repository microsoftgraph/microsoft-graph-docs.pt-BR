# <a name="verifieddomain-resource-type"></a><span data-ttu-id="778d3-101">Tipo de recurso verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="778d3-101">verifiedDomain resource type</span></span>

<span data-ttu-id="778d3-p101">Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="778d3-p101">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="778d3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="778d3-104">Properties</span></span>
| <span data-ttu-id="778d3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="778d3-105">Property</span></span>     | <span data-ttu-id="778d3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="778d3-106">Type</span></span>   |<span data-ttu-id="778d3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="778d3-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="778d3-108">capabilities</span><span class="sxs-lookup"><span data-stu-id="778d3-108">capabilities</span></span>|<span data-ttu-id="778d3-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="778d3-109">String</span></span>|<span data-ttu-id="778d3-110">Por exemplo, "Email" ou "OfficeCommunicationsOnline".</span><span class="sxs-lookup"><span data-stu-id="778d3-110">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="778d3-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="778d3-111">isDefault</span></span>|<span data-ttu-id="778d3-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="778d3-112">Boolean</span></span>|                <span data-ttu-id="778d3-113">**true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="778d3-113">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="778d3-114">isInitial</span><span class="sxs-lookup"><span data-stu-id="778d3-114">isInitial</span></span>|<span data-ttu-id="778d3-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="778d3-115">Boolean</span></span>|<span data-ttu-id="778d3-116">**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**</span><span class="sxs-lookup"><span data-stu-id="778d3-116">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="778d3-117">name</span><span class="sxs-lookup"><span data-stu-id="778d3-117">name</span></span>|<span data-ttu-id="778d3-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="778d3-118">String</span></span>|<span data-ttu-id="778d3-119">O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.</span><span class="sxs-lookup"><span data-stu-id="778d3-119">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="778d3-120">type</span><span class="sxs-lookup"><span data-stu-id="778d3-120">type</span></span>|<span data-ttu-id="778d3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="778d3-121">String</span></span>|<span data-ttu-id="778d3-122">Por exemplo, "Managed".</span><span class="sxs-lookup"><span data-stu-id="778d3-122">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="778d3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="778d3-123">JSON representation</span></span>

<span data-ttu-id="778d3-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="778d3-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
