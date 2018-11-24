# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="104ab-101">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="104ab-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="104ab-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="104ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="104ab-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="104ab-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="104ab-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="104ab-104">Properties</span></span>
|<span data-ttu-id="104ab-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="104ab-105">Property</span></span>|<span data-ttu-id="104ab-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="104ab-106">Type</span></span>|<span data-ttu-id="104ab-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="104ab-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="104ab-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="104ab-108">movieRating</span></span>|[<span data-ttu-id="104ab-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="104ab-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="104ab-110">Filmes selecionado para a Nova Zelândia de classificação.</span><span class="sxs-lookup"><span data-stu-id="104ab-110">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="104ab-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="104ab-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="104ab-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="104ab-112">tvRating</span></span>|[<span data-ttu-id="104ab-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="104ab-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="104ab-114">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="104ab-114">TV rating selected for New Zealand.</span></span> <span data-ttu-id="104ab-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="104ab-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="104ab-116">Relações</span><span class="sxs-lookup"><span data-stu-id="104ab-116">Relationships</span></span>
<span data-ttu-id="104ab-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="104ab-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="104ab-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="104ab-118">JSON Representation</span></span>
<span data-ttu-id="104ab-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="104ab-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



