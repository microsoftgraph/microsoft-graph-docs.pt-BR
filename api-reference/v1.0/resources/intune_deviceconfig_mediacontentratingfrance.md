# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="eb1cb-101">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="eb1cb-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="eb1cb-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb1cb-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb1cb-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="eb1cb-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb1cb-104">Properties</span></span>
|<span data-ttu-id="eb1cb-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb1cb-105">Property</span></span>|<span data-ttu-id="eb1cb-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb1cb-106">Type</span></span>|<span data-ttu-id="eb1cb-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb1cb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb1cb-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="eb1cb-108">movieRating</span></span>|[<span data-ttu-id="eb1cb-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="eb1cb-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="eb1cb-110">Classificações de filmes selecionadas para França.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-110">Movies rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="eb1cb-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-111">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="eb1cb-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="eb1cb-112">tvRating</span></span>|[<span data-ttu-id="eb1cb-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="eb1cb-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="eb1cb-114">Classificação de TV selecionada para França.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-114">TV rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="eb1cb-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-115">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb1cb-116">Relações</span><span class="sxs-lookup"><span data-stu-id="eb1cb-116">Relationships</span></span>
<span data-ttu-id="eb1cb-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb1cb-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb1cb-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb1cb-118">JSON Representation</span></span>
<span data-ttu-id="eb1cb-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb1cb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



