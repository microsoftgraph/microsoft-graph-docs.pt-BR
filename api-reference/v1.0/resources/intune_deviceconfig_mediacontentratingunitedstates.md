# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="8876a-101">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="8876a-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="8876a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8876a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8876a-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8876a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8876a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8876a-104">Properties</span></span>
|<span data-ttu-id="8876a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8876a-105">Property</span></span>|<span data-ttu-id="8876a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8876a-106">Type</span></span>|<span data-ttu-id="8876a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8876a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8876a-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="8876a-108">movieRating</span></span>|[<span data-ttu-id="8876a-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="8876a-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="8876a-110">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="8876a-110">Movies rating selected for United States Possible values are: , , , , , , .</span></span> <span data-ttu-id="8876a-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8876a-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="8876a-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="8876a-112">tvRating</span></span>|[<span data-ttu-id="8876a-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8876a-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="8876a-114">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="8876a-114">TV rating selected for United States Possible values are: , , , , , , , .</span></span> <span data-ttu-id="8876a-115">Os valores possíveis são:  `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8876a-115">The possible values are `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="8876a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8876a-116">Relationships</span></span>
<span data-ttu-id="8876a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8876a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8876a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8876a-118">JSON Representation</span></span>
<span data-ttu-id="8876a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8876a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



