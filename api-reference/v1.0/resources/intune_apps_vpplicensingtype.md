# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="d03b1-101">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="d03b1-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="d03b1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d03b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d03b1-103">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="d03b1-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="d03b1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d03b1-104">Properties</span></span>
|<span data-ttu-id="d03b1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d03b1-105">Property</span></span>|<span data-ttu-id="d03b1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d03b1-106">Type</span></span>|<span data-ttu-id="d03b1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d03b1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d03b1-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="d03b1-108">supportsUserLicensing</span></span>|<span data-ttu-id="d03b1-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="d03b1-109">Boolean</span></span>|<span data-ttu-id="d03b1-110">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="d03b1-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="d03b1-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d03b1-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="d03b1-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="d03b1-112">Boolean</span></span>|<span data-ttu-id="d03b1-113">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d03b1-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d03b1-114">Relações</span><span class="sxs-lookup"><span data-stu-id="d03b1-114">Relationships</span></span>
<span data-ttu-id="d03b1-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d03b1-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d03b1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d03b1-116">JSON Representation</span></span>
<span data-ttu-id="d03b1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d03b1-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



