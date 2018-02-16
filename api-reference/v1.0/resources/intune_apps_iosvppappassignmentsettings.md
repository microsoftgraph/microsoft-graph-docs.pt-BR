# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="a085c-101">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a085c-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a085c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a085c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a085c-103">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a085c-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="a085c-104">Herda de [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a085c-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a085c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a085c-105">Properties</span></span>
|<span data-ttu-id="a085c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a085c-106">Property</span></span>|<span data-ttu-id="a085c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a085c-107">Type</span></span>|<span data-ttu-id="a085c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a085c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a085c-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a085c-109">useDeviceLicensing</span></span>|<span data-ttu-id="a085c-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="a085c-110">Boolean</span></span>|<span data-ttu-id="a085c-111">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a085c-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="a085c-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a085c-112">vpnConfigurationId</span></span>|<span data-ttu-id="a085c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a085c-113">String</span></span>|<span data-ttu-id="a085c-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a085c-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a085c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a085c-115">Relationships</span></span>
<span data-ttu-id="a085c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a085c-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a085c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a085c-117">JSON Representation</span></span>
<span data-ttu-id="a085c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a085c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



