# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="2010d-101">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="2010d-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="2010d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2010d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2010d-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2010d-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2010d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2010d-104">Properties</span></span>
|<span data-ttu-id="2010d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2010d-105">Property</span></span>|<span data-ttu-id="2010d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2010d-106">Type</span></span>|<span data-ttu-id="2010d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2010d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2010d-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2010d-108">movieRating</span></span>|[<span data-ttu-id="2010d-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="2010d-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="2010d-p101">Classificação de filmes selecionada para a Alemanha. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2010d-p101">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="2010d-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="2010d-112">tvRating</span></span>|[<span data-ttu-id="2010d-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2010d-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="2010d-p102">Classificação de TV selecionada para a Alemanha. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2010d-p102">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2010d-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="2010d-116">Relationships</span></span>
<span data-ttu-id="2010d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2010d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2010d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2010d-118">JSON Representation</span></span>
<span data-ttu-id="2010d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2010d-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```








