# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="36a8a-101">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="36a8a-101">recentNotebookLinks resource type</span></span>

<span data-ttu-id="36a8a-102">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="36a8a-102">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="36a8a-103">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="36a8a-103">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="36a8a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36a8a-104">Properties</span></span>
| <span data-ttu-id="36a8a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36a8a-105">Property</span></span>     | <span data-ttu-id="36a8a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="36a8a-106">Type</span></span>   |<span data-ttu-id="36a8a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="36a8a-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36a8a-108">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="36a8a-108">oneNoteClientUrl</span></span>|[<span data-ttu-id="36a8a-109">externalLink</span><span class="sxs-lookup"><span data-stu-id="36a8a-109">externalLink</span></span>](externallink.md)|<span data-ttu-id="36a8a-110">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="36a8a-110">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="36a8a-111">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="36a8a-111">oneNoteWebUrl</span></span>|[<span data-ttu-id="36a8a-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="36a8a-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="36a8a-113">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="36a8a-113">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36a8a-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36a8a-114">JSON representation</span></span>

<span data-ttu-id="36a8a-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36a8a-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
