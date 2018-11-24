# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="6cfbe-101">tipo de recurso de teamsTabConfiguration (Open tipo)</span><span class="sxs-lookup"><span data-stu-id="6cfbe-101">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="6cfbe-102">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-102">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="6cfbe-103">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-103">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="6cfbe-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cfbe-104">Properties</span></span>

|<span data-ttu-id="6cfbe-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cfbe-105">Property</span></span>|<span data-ttu-id="6cfbe-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cfbe-106">Type</span></span>|<span data-ttu-id="6cfbe-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cfbe-107">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="6cfbe-108">entityId</span><span class="sxs-lookup"><span data-stu-id="6cfbe-108">entityId</span></span>   |   <span data-ttu-id="6cfbe-109">string</span><span class="sxs-lookup"><span data-stu-id="6cfbe-109">string</span></span> |  <span data-ttu-id="6cfbe-110">Identificador da entidade hospedados pelo provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-110">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="6cfbe-111">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6cfbe-111">contentUrl</span></span> |   <span data-ttu-id="6cfbe-112">string</span><span class="sxs-lookup"><span data-stu-id="6cfbe-112">string</span></span> |  <span data-ttu-id="6cfbe-113">URL usada para processar o conteúdo da guia em equipes.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-113">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="6cfbe-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-114">Required.</span></span>    |
|  <span data-ttu-id="6cfbe-115">removeUrl</span><span class="sxs-lookup"><span data-stu-id="6cfbe-115">removeUrl</span></span>  |   <span data-ttu-id="6cfbe-116">string</span><span class="sxs-lookup"><span data-stu-id="6cfbe-116">string</span></span> |  <span data-ttu-id="6cfbe-117">Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-117">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="6cfbe-118">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="6cfbe-118">websiteUrl</span></span> |   <span data-ttu-id="6cfbe-119">string</span><span class="sxs-lookup"><span data-stu-id="6cfbe-119">string</span></span> |  <span data-ttu-id="6cfbe-120">URL para a exibição de conteúdo da guia fora equipes.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-120">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="6cfbe-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cfbe-121">JSON representation</span></span>

<span data-ttu-id="6cfbe-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6cfbe-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
