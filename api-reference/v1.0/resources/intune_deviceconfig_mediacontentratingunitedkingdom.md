# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="daa50-101">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="daa50-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="daa50-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="daa50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="daa50-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="daa50-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="daa50-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daa50-104">Properties</span></span>
|<span data-ttu-id="daa50-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daa50-105">Property</span></span>|<span data-ttu-id="daa50-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="daa50-106">Type</span></span>|<span data-ttu-id="daa50-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="daa50-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa50-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="daa50-108">movieRating</span></span>|[<span data-ttu-id="daa50-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="daa50-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="daa50-110">Classificações de filmes selecionadas para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="daa50-110">Movies rating selected for United Kingdom Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="daa50-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="daa50-111">The possible values are `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`, , , or .</span></span>|
|<span data-ttu-id="daa50-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="daa50-112">tvRating</span></span>|[<span data-ttu-id="daa50-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="daa50-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="daa50-114">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="daa50-114">TV rating selected for United Kingdom Possible values are: , , .</span></span> <span data-ttu-id="daa50-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="daa50-115">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="daa50-116">Relações</span><span class="sxs-lookup"><span data-stu-id="daa50-116">Relationships</span></span>
<span data-ttu-id="daa50-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="daa50-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="daa50-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daa50-118">JSON Representation</span></span>
<span data-ttu-id="daa50-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="daa50-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



