# <a name="ipv4range-resource-type"></a><span data-ttu-id="1bd20-101">Tipo de recurso iPv4Range</span><span class="sxs-lookup"><span data-stu-id="1bd20-101">iPv4Range resource type</span></span>

> <span data-ttu-id="1bd20-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1bd20-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bd20-103">Intervalo de IP V4</span><span class="sxs-lookup"><span data-stu-id="1bd20-103">IP V4 range</span></span>

<span data-ttu-id="1bd20-104">Herda de [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1bd20-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1bd20-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bd20-105">Properties</span></span>
|<span data-ttu-id="1bd20-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bd20-106">Property</span></span>|<span data-ttu-id="1bd20-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd20-107">Type</span></span>|<span data-ttu-id="1bd20-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd20-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd20-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="1bd20-109">lowerAddress</span></span>|<span data-ttu-id="1bd20-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd20-110">String</span></span>|<span data-ttu-id="1bd20-111">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="1bd20-111">Lower IP Address</span></span>|
|<span data-ttu-id="1bd20-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="1bd20-112">upperAddress</span></span>|<span data-ttu-id="1bd20-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd20-113">String</span></span>|<span data-ttu-id="1bd20-114">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="1bd20-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bd20-115">Relações</span><span class="sxs-lookup"><span data-stu-id="1bd20-115">Relationships</span></span>
<span data-ttu-id="1bd20-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1bd20-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1bd20-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bd20-117">JSON Representation</span></span>
<span data-ttu-id="1bd20-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bd20-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.ipRange",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



