# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="3cfa7-101">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3cfa7-101">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="3cfa7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cfa7-103">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-103">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="3cfa7-104">Herda de [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3cfa7-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3cfa7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cfa7-105">Properties</span></span>
|<span data-ttu-id="3cfa7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cfa7-106">Property</span></span>|<span data-ttu-id="3cfa7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cfa7-107">Type</span></span>|<span data-ttu-id="3cfa7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cfa7-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfa7-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="3cfa7-109">vpnConfigurationId</span></span>|<span data-ttu-id="3cfa7-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cfa7-110">String</span></span>|<span data-ttu-id="3cfa7-111">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cfa7-112">Relações</span><span class="sxs-lookup"><span data-stu-id="3cfa7-112">Relationships</span></span>
<span data-ttu-id="3cfa7-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3cfa7-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3cfa7-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cfa7-114">JSON Representation</span></span>
<span data-ttu-id="3cfa7-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



