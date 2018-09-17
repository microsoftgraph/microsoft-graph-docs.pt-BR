# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a8568-101">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a8568-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="a8568-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8568-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8568-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8568-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a8568-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8568-104">Properties</span></span>
|<span data-ttu-id="a8568-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8568-105">Property</span></span>|<span data-ttu-id="a8568-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8568-106">Type</span></span>|<span data-ttu-id="a8568-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8568-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8568-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="a8568-108">movieRating</span></span>|[<span data-ttu-id="a8568-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="a8568-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="a8568-110">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="a8568-110">Movies rating selected for Ireland Possible values are: , , , , , , , .</span></span> <span data-ttu-id="a8568-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a8568-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a8568-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="a8568-112">tvRating</span></span>|[<span data-ttu-id="a8568-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a8568-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="a8568-114">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="a8568-114">TV rating selected for Ireland Possible values are: , , , , , , .</span></span> <span data-ttu-id="a8568-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a8568-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8568-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a8568-116">Relationships</span></span>
<span data-ttu-id="a8568-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8568-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8568-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8568-118">JSON Representation</span></span>
<span data-ttu-id="a8568-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8568-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```








