# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c7276-101">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c7276-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="c7276-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7276-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7276-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7276-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c7276-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7276-104">Properties</span></span>
|<span data-ttu-id="c7276-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7276-105">Property</span></span>|<span data-ttu-id="c7276-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7276-106">Type</span></span>|<span data-ttu-id="c7276-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7276-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7276-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c7276-108">movieRating</span></span>|[<span data-ttu-id="c7276-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c7276-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="c7276-p101">Classificação de filmes selecionada para a Austrália. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c7276-p101">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c7276-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c7276-112">tvRating</span></span>|[<span data-ttu-id="c7276-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c7276-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="c7276-p102">Classificação de filmes selecionada para a Austrália. Os valores possíveis são: `allAllowed` `allBlocked` `preschoolers` `children` `general` `parentalGuidance` `mature` `agesAbove15` `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c7276-p102">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7276-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c7276-116">Relationships</span></span>
<span data-ttu-id="c7276-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7276-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7276-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7276-118">JSON Representation</span></span>
<span data-ttu-id="c7276-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7276-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```








