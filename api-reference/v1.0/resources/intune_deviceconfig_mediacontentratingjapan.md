# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="cc655-101">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="cc655-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="cc655-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cc655-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc655-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cc655-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cc655-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc655-104">Properties</span></span>
|<span data-ttu-id="cc655-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc655-105">Property</span></span>|<span data-ttu-id="cc655-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc655-106">Type</span></span>|<span data-ttu-id="cc655-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc655-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc655-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="cc655-108">movieRating</span></span>|[<span data-ttu-id="cc655-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="cc655-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="cc655-p101">Classificação de filmes selecionada para o Japão. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cc655-p101">Movies rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cc655-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="cc655-112">tvRating</span></span>|[<span data-ttu-id="cc655-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cc655-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="cc655-p102">Classificação de TV selecionada para o Japão. Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="cc655-p102">TV rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc655-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="cc655-116">Relationships</span></span>
<span data-ttu-id="cc655-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc655-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc655-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc655-118">JSON Representation</span></span>
<span data-ttu-id="cc655-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc655-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```








