# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c0d8d-101">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c0d8d-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="c0d8d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0d8d-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c0d8d-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c0d8d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0d8d-104">Properties</span></span>
|<span data-ttu-id="c0d8d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0d8d-105">Property</span></span>|<span data-ttu-id="c0d8d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0d8d-106">Type</span></span>|<span data-ttu-id="c0d8d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0d8d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0d8d-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c0d8d-108">movieRating</span></span>|[<span data-ttu-id="c0d8d-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c0d8d-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="c0d8d-110">Classificações de filmes selecionadas para Austrália.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-110">Movies rating selected for Australia Possible values are: , , , , , , .</span></span> <span data-ttu-id="c0d8d-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`, , , , , or .</span></span>|
|<span data-ttu-id="c0d8d-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c0d8d-112">tvRating</span></span>|[<span data-ttu-id="c0d8d-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c0d8d-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="c0d8d-114">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-114">TV rating selected for Australia Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="c0d8d-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-115">The possible values are `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`, , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0d8d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c0d8d-116">Relationships</span></span>
<span data-ttu-id="c0d8d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0d8d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0d8d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0d8d-118">JSON Representation</span></span>
<span data-ttu-id="c0d8d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0d8d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



