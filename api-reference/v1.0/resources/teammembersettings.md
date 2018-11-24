# <a name="teammembersettings-resource-type"></a><span data-ttu-id="b4283-101">tipo de recurso de teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b4283-101">teamMemberSettings resource type</span></span>



<span data-ttu-id="b4283-102">Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="b4283-102">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4283-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4283-103">Properties</span></span>
| <span data-ttu-id="b4283-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4283-104">Property</span></span>     | <span data-ttu-id="b4283-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4283-105">Type</span></span>   |<span data-ttu-id="b4283-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4283-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4283-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b4283-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b4283-108">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4283-108">Boolean</span></span>|<span data-ttu-id="b4283-109">Se definido como true, membros pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="b4283-109">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="b4283-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b4283-110">allowDeleteChannels</span></span>|<span data-ttu-id="b4283-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4283-111">Boolean</span></span>|<span data-ttu-id="b4283-112">Se definido como true, membros pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="b4283-112">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="b4283-113">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="b4283-113">allowAddRemoveApps</span></span>|<span data-ttu-id="b4283-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4283-114">Boolean</span></span>|<span data-ttu-id="b4283-115">Se definido como true, membros pode adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b4283-115">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="b4283-116">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="b4283-116">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="b4283-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4283-117">Boolean</span></span>|<span data-ttu-id="b4283-118">Se definido como true, membros pode adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="b4283-118">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="b4283-119">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="b4283-119">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="b4283-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4283-120">Boolean</span></span>|<span data-ttu-id="b4283-121">Se definido como true, membros pode adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="b4283-121">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4283-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4283-122">JSON representation</span></span>

<span data-ttu-id="b4283-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4283-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
