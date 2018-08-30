# <a name="baseitemversion-resource-type"></a><span data-ttu-id="7335b-101">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="7335b-101">BaseItemVersion resource type</span></span>

<span data-ttu-id="7335b-102">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="7335b-102">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7335b-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7335b-103">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="7335b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7335b-104">Properties</span></span>

|      <span data-ttu-id="7335b-105">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7335b-105">Property name</span></span>       |                         <span data-ttu-id="7335b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="7335b-106">Type</span></span>                         |                               <span data-ttu-id="7335b-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="7335b-107">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="7335b-108">**id**</span><span class="sxs-lookup"><span data-stu-id="7335b-108">**id**</span></span>                   | <span data-ttu-id="7335b-109">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="7335b-109">string</span></span>                                               | <span data-ttu-id="7335b-110">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="7335b-110">The ID of the version.</span></span> <span data-ttu-id="7335b-111">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7335b-111">Read-only.</span></span>                                       |
| <span data-ttu-id="7335b-112">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="7335b-112">**lastModifiedBy**</span></span>       | [<span data-ttu-id="7335b-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7335b-113">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="7335b-114">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7335b-114">Identity of the user which last modified the version.</span></span> <span data-ttu-id="7335b-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7335b-115">Read-only.</span></span>        |
| <span data-ttu-id="7335b-116">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7335b-116">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="7335b-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7335b-117">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="7335b-118">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7335b-118">Date and time the version was last modified.</span></span> <span data-ttu-id="7335b-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7335b-119">Read-only.</span></span>                 |
| <span data-ttu-id="7335b-120">**publication**</span><span class="sxs-lookup"><span data-stu-id="7335b-120">**publication**</span></span>          | [<span data-ttu-id="7335b-121">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="7335b-121">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="7335b-122">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="7335b-122">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="7335b-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7335b-123">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
