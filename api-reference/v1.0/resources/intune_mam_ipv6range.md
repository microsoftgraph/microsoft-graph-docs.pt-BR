# <a name="ipv6range-resource-type"></a><span data-ttu-id="2d43c-101">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="2d43c-101">iPv6Range resource type</span></span>

> <span data-ttu-id="2d43c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d43c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d43c-103">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="2d43c-103">IP V6 range</span></span>

<span data-ttu-id="2d43c-104">Herda de [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="2d43c-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2d43c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d43c-105">Properties</span></span>
|<span data-ttu-id="2d43c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d43c-106">Property</span></span>|<span data-ttu-id="2d43c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d43c-107">Type</span></span>|<span data-ttu-id="2d43c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d43c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d43c-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2d43c-109">lowerAddress</span></span>|<span data-ttu-id="2d43c-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d43c-110">String</span></span>|<span data-ttu-id="2d43c-111">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="2d43c-111">Lower IP Address</span></span>|
|<span data-ttu-id="2d43c-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2d43c-112">upperAddress</span></span>|<span data-ttu-id="2d43c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d43c-113">String</span></span>|<span data-ttu-id="2d43c-114">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="2d43c-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d43c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2d43c-115">Relationships</span></span>
<span data-ttu-id="2d43c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d43c-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d43c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d43c-117">JSON Representation</span></span>
<span data-ttu-id="2d43c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d43c-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```








