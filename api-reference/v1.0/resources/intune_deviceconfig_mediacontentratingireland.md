# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="c5694-101">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="c5694-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="c5694-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5694-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5694-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c5694-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c5694-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5694-104">Properties</span></span>
|<span data-ttu-id="c5694-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5694-105">Property</span></span>|<span data-ttu-id="c5694-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5694-106">Type</span></span>|<span data-ttu-id="c5694-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5694-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5694-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c5694-108">movieRating</span></span>|<span data-ttu-id="c5694-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5694-109">String</span></span>|<span data-ttu-id="c5694-110">Classificação de filmes selecionada para a Irlanda Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c5694-110">Movies rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c5694-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="c5694-111">tvRating</span></span>|<span data-ttu-id="c5694-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5694-112">String</span></span>|<span data-ttu-id="c5694-113">Classificação de TV selecionada para a Irlanda Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="c5694-113">TV rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5694-114">Relações</span><span class="sxs-lookup"><span data-stu-id="c5694-114">Relationships</span></span>
<span data-ttu-id="c5694-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5694-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5694-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5694-116">JSON Representation</span></span>
<span data-ttu-id="c5694-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5694-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



