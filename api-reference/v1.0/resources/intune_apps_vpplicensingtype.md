# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8fa2f-101">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="8fa2f-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="8fa2f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fa2f-103">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="8fa2f-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="8fa2f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fa2f-104">Properties</span></span>
|<span data-ttu-id="8fa2f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fa2f-105">Property</span></span>|<span data-ttu-id="8fa2f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fa2f-106">Type</span></span>|<span data-ttu-id="8fa2f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fa2f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fa2f-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8fa2f-108">supportsUserLicensing</span></span>|<span data-ttu-id="8fa2f-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="8fa2f-109">Boolean</span></span>|<span data-ttu-id="8fa2f-110">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8fa2f-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8fa2f-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="8fa2f-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="8fa2f-112">Boolean</span></span>|<span data-ttu-id="8fa2f-113">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fa2f-114">Relações</span><span class="sxs-lookup"><span data-stu-id="8fa2f-114">Relationships</span></span>
<span data-ttu-id="8fa2f-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fa2f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fa2f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fa2f-116">JSON Representation</span></span>
<span data-ttu-id="8fa2f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



