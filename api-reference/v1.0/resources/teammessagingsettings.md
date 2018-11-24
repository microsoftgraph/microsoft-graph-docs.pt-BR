# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="7b877-101">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="7b877-101">teamMessagingSettings resource type</span></span>



<span data-ttu-id="7b877-102">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="7b877-102">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7b877-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b877-103">Properties</span></span>
| <span data-ttu-id="7b877-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b877-104">Property</span></span>     | <span data-ttu-id="7b877-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b877-105">Type</span></span>   |<span data-ttu-id="7b877-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b877-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b877-107">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="7b877-107">allowUserEditMessages</span></span>|<span data-ttu-id="7b877-108">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b877-108">Boolean</span></span>|<span data-ttu-id="7b877-109">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7b877-109">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="7b877-110">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7b877-110">allowUserDeleteMessages</span></span>|<span data-ttu-id="7b877-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b877-111">Boolean</span></span>|<span data-ttu-id="7b877-112">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7b877-112">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="7b877-113">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7b877-113">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="7b877-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b877-114">Boolean</span></span>|<span data-ttu-id="7b877-115">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="7b877-115">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="7b877-116">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="7b877-116">allowTeamMentions</span></span>|<span data-ttu-id="7b877-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b877-117">Boolean</span></span>|<span data-ttu-id="7b877-118">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7b877-118">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="7b877-119">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="7b877-119">allowChannelMentions</span></span>|<span data-ttu-id="7b877-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b877-120">Boolean</span></span>|<span data-ttu-id="7b877-121">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7b877-121">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b877-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b877-122">JSON representation</span></span>

<span data-ttu-id="7b877-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b877-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
