# <a name="educationterm-resource-type"></a><span data-ttu-id="0b42d-101">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="0b42d-101">educationTerm resource type</span></span>

<span data-ttu-id="0b42d-102">Termo A.</span><span class="sxs-lookup"><span data-stu-id="0b42d-102">A term.</span></span> <span data-ttu-id="0b42d-103">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="0b42d-103">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="0b42d-104">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="0b42d-104">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0b42d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b42d-105">Properties</span></span>
| <span data-ttu-id="0b42d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b42d-106">Property</span></span>     | <span data-ttu-id="0b42d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b42d-107">Type</span></span>   |<span data-ttu-id="0b42d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b42d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b42d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0b42d-109">displayName</span></span>| <span data-ttu-id="0b42d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b42d-110">String</span></span>| <span data-ttu-id="0b42d-111">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="0b42d-111">Display name of the template.</span></span>| 
|<span data-ttu-id="0b42d-112">externalId</span><span class="sxs-lookup"><span data-stu-id="0b42d-112">externalId</span></span>|<span data-ttu-id="0b42d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b42d-113">String</span></span>| <span data-ttu-id="0b42d-114">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b42d-114">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="0b42d-115">startDate</span><span class="sxs-lookup"><span data-stu-id="0b42d-115">startDate</span></span>|<span data-ttu-id="0b42d-116">Data</span><span class="sxs-lookup"><span data-stu-id="0b42d-116">Date</span></span>|<span data-ttu-id="0b42d-117">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="0b42d-117">Start of the term.</span></span>|
|<span data-ttu-id="0b42d-118">endDate</span><span class="sxs-lookup"><span data-stu-id="0b42d-118">endDate</span></span>|<span data-ttu-id="0b42d-119">Data</span><span class="sxs-lookup"><span data-stu-id="0b42d-119">Date</span></span>|<span data-ttu-id="0b42d-120">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="0b42d-120">End of the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b42d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b42d-121">JSON representation</span></span>

<span data-ttu-id="0b42d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b42d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->