# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="ecf5e-101">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ecf5e-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="ecf5e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecf5e-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ecf5e-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ecf5e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecf5e-104">Properties</span></span>
|<span data-ttu-id="ecf5e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecf5e-105">Property</span></span>|<span data-ttu-id="ecf5e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecf5e-106">Type</span></span>|<span data-ttu-id="ecf5e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecf5e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf5e-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ecf5e-108">movieRating</span></span>|[<span data-ttu-id="ecf5e-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="ecf5e-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="ecf5e-110">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-110">Movies rating selected for Canada Possible values are: , , , , , , .</span></span> <span data-ttu-id="ecf5e-111">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`, , , , , or .</span></span>|
|<span data-ttu-id="ecf5e-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="ecf5e-112">tvRating</span></span>|[<span data-ttu-id="ecf5e-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ecf5e-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="ecf5e-114">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-114">TV rating selected for Canada Possible values are: , , , , , , , .</span></span> <span data-ttu-id="ecf5e-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-115">The possible values are `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecf5e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ecf5e-116">Relationships</span></span>
<span data-ttu-id="ecf5e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecf5e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecf5e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecf5e-118">JSON Representation</span></span>
<span data-ttu-id="ecf5e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecf5e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



