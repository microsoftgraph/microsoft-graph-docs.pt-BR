# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="66510-101">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="66510-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="66510-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66510-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66510-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="66510-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="66510-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66510-104">Properties</span></span>
|<span data-ttu-id="66510-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66510-105">Property</span></span>|<span data-ttu-id="66510-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="66510-106">Type</span></span>|<span data-ttu-id="66510-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="66510-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66510-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="66510-108">movieRating</span></span>|<span data-ttu-id="66510-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66510-109">String</span></span>|<span data-ttu-id="66510-110">Classificação de filmes selecionada para os Estados Unidos Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="66510-110">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="66510-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="66510-111">tvRating</span></span>|<span data-ttu-id="66510-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66510-112">String</span></span>|<span data-ttu-id="66510-113">Classificação de TV selecionada para os Estados Unidos Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="66510-113">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66510-114">Relações</span><span class="sxs-lookup"><span data-stu-id="66510-114">Relationships</span></span>
<span data-ttu-id="66510-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66510-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66510-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66510-116">JSON Representation</span></span>
<span data-ttu-id="66510-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66510-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



