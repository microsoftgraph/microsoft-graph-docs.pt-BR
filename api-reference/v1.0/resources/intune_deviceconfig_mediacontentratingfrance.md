# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="2626d-101">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="2626d-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="2626d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2626d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2626d-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2626d-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2626d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2626d-104">Properties</span></span>
|<span data-ttu-id="2626d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2626d-105">Property</span></span>|<span data-ttu-id="2626d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2626d-106">Type</span></span>|<span data-ttu-id="2626d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2626d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2626d-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2626d-108">movieRating</span></span>|[<span data-ttu-id="2626d-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="2626d-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="2626d-p101">Classificação de filmes selecionada para a França. Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="2626d-p101">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="2626d-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="2626d-112">tvRating</span></span>|[<span data-ttu-id="2626d-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2626d-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="2626d-p102">Classificação de TV selecionada para a França Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="2626d-p102">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2626d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2626d-116">Relationships</span></span>
<span data-ttu-id="2626d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2626d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2626d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2626d-118">JSON Representation</span></span>
<span data-ttu-id="2626d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2626d-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```








