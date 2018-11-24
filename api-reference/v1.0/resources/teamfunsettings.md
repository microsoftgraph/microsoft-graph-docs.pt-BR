# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="e3ce2-101">tipo de recurso de teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e3ce2-101">teamFunSettings resource type</span></span>



<span data-ttu-id="e3ce2-102">Configurações para configurar o uso de Giphy, adesivos e memes em [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="e3ce2-102">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e3ce2-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3ce2-103">Properties</span></span>
| <span data-ttu-id="e3ce2-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3ce2-104">Property</span></span>     | <span data-ttu-id="e3ce2-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3ce2-105">Type</span></span>   |<span data-ttu-id="e3ce2-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ce2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ce2-107">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="e3ce2-107">allowGiphy</span></span>|<span data-ttu-id="e3ce2-108">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3ce2-108">Boolean</span></span>|<span data-ttu-id="e3ce2-109">Se definido como true, permite que o uso de Giphy.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-109">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="e3ce2-110">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="e3ce2-110">giphyContentRating</span></span>|<span data-ttu-id="e3ce2-111">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="e3ce2-111">String (enum)</span></span>|<span data-ttu-id="e3ce2-112">Classificação de conteúdo Giphy.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-112">Giphy content rating.</span></span> <span data-ttu-id="e3ce2-113">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-113">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="e3ce2-114">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="e3ce2-114">allowStickersAndMemes</span></span>|<span data-ttu-id="e3ce2-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3ce2-115">Boolean</span></span>|<span data-ttu-id="e3ce2-116">Se definido como true, permite que os usuários incluem adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-116">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="e3ce2-117">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="e3ce2-117">allowCustomMemes</span></span>|<span data-ttu-id="e3ce2-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3ce2-118">Boolean</span></span>|<span data-ttu-id="e3ce2-119">Se definido como true, permite que os usuários incluem memes personalizado.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-119">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3ce2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3ce2-120">JSON representation</span></span>

<span data-ttu-id="e3ce2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3ce2-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
