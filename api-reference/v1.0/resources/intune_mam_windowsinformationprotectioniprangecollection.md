# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="842c4-101">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="842c4-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="842c4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="842c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="842c4-103">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="842c4-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="842c4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="842c4-104">Properties</span></span>
|<span data-ttu-id="842c4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="842c4-105">Property</span></span>|<span data-ttu-id="842c4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="842c4-106">Type</span></span>|<span data-ttu-id="842c4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="842c4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842c4-108">displayName</span><span class="sxs-lookup"><span data-stu-id="842c4-108">displayName</span></span>|<span data-ttu-id="842c4-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="842c4-109">String</span></span>|<span data-ttu-id="842c4-110">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="842c4-110">Display name</span></span>|
|<span data-ttu-id="842c4-111">ranges</span><span class="sxs-lookup"><span data-stu-id="842c4-111">ranges</span></span>|<span data-ttu-id="842c4-112">Coleção [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="842c4-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="842c4-113">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="842c4-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="842c4-114">Relações</span><span class="sxs-lookup"><span data-stu-id="842c4-114">Relationships</span></span>
<span data-ttu-id="842c4-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="842c4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="842c4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="842c4-116">JSON Representation</span></span>
<span data-ttu-id="842c4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="842c4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



