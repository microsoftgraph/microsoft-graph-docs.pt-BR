# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="95b63-101">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="95b63-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="95b63-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="95b63-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95b63-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95b63-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="95b63-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95b63-104">Properties</span></span>
|<span data-ttu-id="95b63-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95b63-105">Property</span></span>|<span data-ttu-id="95b63-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="95b63-106">Type</span></span>|<span data-ttu-id="95b63-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b63-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b63-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="95b63-108">movieRating</span></span>|[<span data-ttu-id="95b63-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="95b63-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="95b63-110">Filmes selecionado para Irlanda de classificação.</span><span class="sxs-lookup"><span data-stu-id="95b63-110">Movies rating selected for Ireland.</span></span> <span data-ttu-id="95b63-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="95b63-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="95b63-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="95b63-112">tvRating</span></span>|[<span data-ttu-id="95b63-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="95b63-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="95b63-114">Classificação de TV selecionada para Irlanda.</span><span class="sxs-lookup"><span data-stu-id="95b63-114">TV rating selected for Ireland.</span></span> <span data-ttu-id="95b63-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="95b63-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95b63-116">Relações</span><span class="sxs-lookup"><span data-stu-id="95b63-116">Relationships</span></span>
<span data-ttu-id="95b63-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95b63-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95b63-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95b63-118">JSON Representation</span></span>
<span data-ttu-id="95b63-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95b63-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



