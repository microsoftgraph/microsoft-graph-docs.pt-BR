# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="98a6e-101">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="98a6e-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="98a6e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98a6e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98a6e-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98a6e-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="98a6e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98a6e-104">Properties</span></span>
|<span data-ttu-id="98a6e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98a6e-105">Property</span></span>|<span data-ttu-id="98a6e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="98a6e-106">Type</span></span>|<span data-ttu-id="98a6e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="98a6e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a6e-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="98a6e-108">movieRating</span></span>|[<span data-ttu-id="98a6e-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="98a6e-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="98a6e-p101">Classificação de filmes selecionada para o Reino Unido. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="98a6e-p101">Movies rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="98a6e-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="98a6e-112">tvRating</span></span>|[<span data-ttu-id="98a6e-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="98a6e-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="98a6e-p102">Classificação de TV selecionada para o Reino Unido. Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="98a6e-p102">TV rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98a6e-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="98a6e-116">Relationships</span></span>
<span data-ttu-id="98a6e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98a6e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98a6e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98a6e-118">JSON Representation</span></span>
<span data-ttu-id="98a6e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98a6e-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```








