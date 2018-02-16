# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="be246-101">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="be246-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="be246-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="be246-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be246-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be246-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="be246-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be246-104">Properties</span></span>
|<span data-ttu-id="be246-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be246-105">Property</span></span>|<span data-ttu-id="be246-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="be246-106">Type</span></span>|<span data-ttu-id="be246-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="be246-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be246-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="be246-108">movieRating</span></span>|<span data-ttu-id="be246-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be246-109">String</span></span>|<span data-ttu-id="be246-110">Classificação de filmes selecionada para o Reino Unido Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="be246-110">Movies rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="be246-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="be246-111">tvRating</span></span>|<span data-ttu-id="be246-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be246-112">String</span></span>|<span data-ttu-id="be246-113">Classificação de TV selecionada para o Reino Unido Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="be246-113">TV rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be246-114">Relações</span><span class="sxs-lookup"><span data-stu-id="be246-114">Relationships</span></span>
<span data-ttu-id="be246-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be246-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be246-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be246-116">JSON Representation</span></span>
<span data-ttu-id="be246-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be246-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



