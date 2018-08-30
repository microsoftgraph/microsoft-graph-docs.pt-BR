# <a name="publicationfacet-resource-type"></a><span data-ttu-id="8da45-101">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8da45-101">PublicationFacet resource type</span></span>

<span data-ttu-id="8da45-102">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8da45-102">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8da45-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8da45-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8da45-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8da45-104">Properties</span></span>

|   <span data-ttu-id="8da45-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8da45-105">Property</span></span>    |  <span data-ttu-id="8da45-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8da45-106">Type</span></span>  | <span data-ttu-id="8da45-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da45-107">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="8da45-108">**level**</span><span class="sxs-lookup"><span data-stu-id="8da45-108">**level**</span></span>     | <span data-ttu-id="8da45-109">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da45-109">String</span></span> | <span data-ttu-id="8da45-110">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="8da45-110">The state of publication for this document.</span></span> <span data-ttu-id="8da45-111">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="8da45-111">Either `published` or `checkout`.</span></span> <span data-ttu-id="8da45-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8da45-112">Read-only.</span></span>  |
| <span data-ttu-id="8da45-113">**versionId**</span><span class="sxs-lookup"><span data-stu-id="8da45-113">**versionId**</span></span> | <span data-ttu-id="8da45-114">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da45-114">String</span></span> | <span data-ttu-id="8da45-115">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="8da45-115">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="8da45-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8da45-116">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
