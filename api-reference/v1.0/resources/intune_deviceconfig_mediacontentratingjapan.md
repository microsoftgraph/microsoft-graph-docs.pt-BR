# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="6c482-101">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6c482-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="6c482-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6c482-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c482-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c482-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6c482-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c482-104">Properties</span></span>
|<span data-ttu-id="6c482-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c482-105">Property</span></span>|<span data-ttu-id="6c482-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c482-106">Type</span></span>|<span data-ttu-id="6c482-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c482-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c482-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="6c482-108">movieRating</span></span>|[<span data-ttu-id="6c482-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="6c482-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="6c482-110">Filmes classificação selecionado para japonês.</span><span class="sxs-lookup"><span data-stu-id="6c482-110">Movies rating selected for Japan.</span></span> <span data-ttu-id="6c482-111">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6c482-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="6c482-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="6c482-112">tvRating</span></span>|[<span data-ttu-id="6c482-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6c482-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="6c482-114">Classificação de TV selecionada para japonês.</span><span class="sxs-lookup"><span data-stu-id="6c482-114">TV rating selected for Japan.</span></span> <span data-ttu-id="6c482-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="6c482-115">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c482-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="6c482-116">Relationships</span></span>
<span data-ttu-id="6c482-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c482-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c482-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c482-118">JSON Representation</span></span>
<span data-ttu-id="6c482-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c482-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



