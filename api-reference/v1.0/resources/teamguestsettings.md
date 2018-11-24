# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="21e52-101">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="21e52-101">teamGuestSettings resource type</span></span>



<span data-ttu-id="21e52-102">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="21e52-102">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21e52-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21e52-103">Properties</span></span>
| <span data-ttu-id="21e52-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21e52-104">Property</span></span>     | <span data-ttu-id="21e52-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="21e52-105">Type</span></span>   |<span data-ttu-id="21e52-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e52-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21e52-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="21e52-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="21e52-108">Booliano</span><span class="sxs-lookup"><span data-stu-id="21e52-108">Boolean</span></span>|<span data-ttu-id="21e52-109">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="21e52-109">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="21e52-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="21e52-110">allowDeleteChannels</span></span>|<span data-ttu-id="21e52-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="21e52-111">Boolean</span></span>|<span data-ttu-id="21e52-112">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="21e52-112">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21e52-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21e52-113">JSON representation</span></span>

<span data-ttu-id="21e52-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21e52-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
