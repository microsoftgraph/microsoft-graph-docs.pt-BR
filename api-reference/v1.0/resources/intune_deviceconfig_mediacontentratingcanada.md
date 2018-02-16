# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="e5457-101">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="e5457-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="e5457-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e5457-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5457-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e5457-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e5457-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5457-104">Properties</span></span>
|<span data-ttu-id="e5457-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5457-105">Property</span></span>|<span data-ttu-id="e5457-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5457-106">Type</span></span>|<span data-ttu-id="e5457-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5457-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5457-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="e5457-108">movieRating</span></span>|<span data-ttu-id="e5457-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5457-109">String</span></span>|<span data-ttu-id="e5457-110">Classificação de filmes selecionada para o Canadá Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="e5457-110">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="e5457-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="e5457-111">tvRating</span></span>|<span data-ttu-id="e5457-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5457-112">String</span></span>|<span data-ttu-id="e5457-113">Classificação de TV selecionada para o Canadá Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e5457-113">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5457-114">Relações</span><span class="sxs-lookup"><span data-stu-id="e5457-114">Relationships</span></span>
<span data-ttu-id="e5457-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5457-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5457-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5457-116">JSON Representation</span></span>
<span data-ttu-id="e5457-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5457-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



