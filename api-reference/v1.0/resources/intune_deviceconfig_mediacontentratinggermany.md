# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="701d8-101">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="701d8-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="701d8-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="701d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="701d8-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="701d8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="701d8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="701d8-104">Properties</span></span>
|<span data-ttu-id="701d8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="701d8-105">Property</span></span>|<span data-ttu-id="701d8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="701d8-106">Type</span></span>|<span data-ttu-id="701d8-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="701d8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="701d8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="701d8-108">movieRating</span></span>|[<span data-ttu-id="701d8-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="701d8-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="701d8-110">Classificação de filmes selecionados para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="701d8-110">Movies rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="701d8-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="701d8-111">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="701d8-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="701d8-112">tvRating</span></span>|[<span data-ttu-id="701d8-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="701d8-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="701d8-114">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="701d8-114">TV rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="701d8-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="701d8-115">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="701d8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="701d8-116">Relationships</span></span>
<span data-ttu-id="701d8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="701d8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="701d8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="701d8-118">JSON Representation</span></span>
<span data-ttu-id="701d8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="701d8-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



