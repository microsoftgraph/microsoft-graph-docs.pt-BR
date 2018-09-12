# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="0730d-101">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="0730d-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="0730d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0730d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0730d-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0730d-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0730d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0730d-104">Properties</span></span>
|<span data-ttu-id="0730d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0730d-105">Property</span></span>|<span data-ttu-id="0730d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="0730d-106">Type</span></span>|<span data-ttu-id="0730d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0730d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0730d-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="0730d-108">movieRating</span></span>|[<span data-ttu-id="0730d-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="0730d-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="0730d-p101">Classificação de filmes selecionada para os Estados Unidos. Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="0730d-p101">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="0730d-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="0730d-112">tvRating</span></span>|[<span data-ttu-id="0730d-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0730d-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="0730d-p102">Classificação de TV selecionada para os Estados Unidos. Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="0730d-p102">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0730d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0730d-116">Relationships</span></span>
<span data-ttu-id="0730d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0730d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0730d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0730d-118">JSON Representation</span></span>
<span data-ttu-id="0730d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0730d-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```








