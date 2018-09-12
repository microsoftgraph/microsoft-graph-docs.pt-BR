# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="18d2c-101">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="18d2c-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="18d2c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18d2c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18d2c-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="18d2c-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="18d2c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18d2c-104">Properties</span></span>
|<span data-ttu-id="18d2c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d2c-105">Property</span></span>|<span data-ttu-id="18d2c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d2c-106">Type</span></span>|<span data-ttu-id="18d2c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d2c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d2c-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="18d2c-108">movieRating</span></span>|[<span data-ttu-id="18d2c-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="18d2c-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="18d2c-p101">Classificação de filmes selecionada para a Nova Zelândia. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="18d2c-p101">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="18d2c-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="18d2c-112">tvRating</span></span>|[<span data-ttu-id="18d2c-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="18d2c-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="18d2c-p102">Classificação de TV selecionada para a Nova Zelândia Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="18d2c-p102">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18d2c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="18d2c-116">Relationships</span></span>
<span data-ttu-id="18d2c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18d2c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18d2c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18d2c-118">JSON Representation</span></span>
<span data-ttu-id="18d2c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18d2c-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








