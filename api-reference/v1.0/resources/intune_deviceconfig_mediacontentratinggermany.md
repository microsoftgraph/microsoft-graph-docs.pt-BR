# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="d6485-101">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d6485-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="d6485-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6485-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6485-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6485-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d6485-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6485-104">Properties</span></span>
|<span data-ttu-id="d6485-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6485-105">Property</span></span>|<span data-ttu-id="d6485-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6485-106">Type</span></span>|<span data-ttu-id="d6485-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6485-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6485-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="d6485-108">movieRating</span></span>|<span data-ttu-id="d6485-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6485-109">String</span></span>|<span data-ttu-id="d6485-110">Classificação de filmes selecionada para a Alemanha Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d6485-110">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d6485-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="d6485-111">tvRating</span></span>|<span data-ttu-id="d6485-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6485-112">String</span></span>|<span data-ttu-id="d6485-113">Classificação de TV selecionada para a Alemanha Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d6485-113">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6485-114">Relações</span><span class="sxs-lookup"><span data-stu-id="d6485-114">Relationships</span></span>
<span data-ttu-id="d6485-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6485-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6485-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6485-116">JSON Representation</span></span>
<span data-ttu-id="d6485-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6485-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



