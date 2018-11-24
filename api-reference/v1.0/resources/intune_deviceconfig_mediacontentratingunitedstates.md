# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="1ef13-101">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1ef13-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="1ef13-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ef13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ef13-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ef13-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1ef13-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ef13-104">Properties</span></span>
|<span data-ttu-id="1ef13-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ef13-105">Property</span></span>|<span data-ttu-id="1ef13-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ef13-106">Type</span></span>|<span data-ttu-id="1ef13-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef13-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef13-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="1ef13-108">movieRating</span></span>|[<span data-ttu-id="1ef13-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="1ef13-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="1ef13-110">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="1ef13-110">Movies rating selected for United States.</span></span> <span data-ttu-id="1ef13-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1ef13-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="1ef13-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="1ef13-112">tvRating</span></span>|[<span data-ttu-id="1ef13-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1ef13-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="1ef13-114">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="1ef13-114">TV rating selected for United States.</span></span> <span data-ttu-id="1ef13-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1ef13-115">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ef13-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1ef13-116">Relationships</span></span>
<span data-ttu-id="1ef13-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ef13-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ef13-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ef13-118">JSON Representation</span></span>
<span data-ttu-id="1ef13-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ef13-119">Here is a JSON representation of the resource.</span></span>
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



