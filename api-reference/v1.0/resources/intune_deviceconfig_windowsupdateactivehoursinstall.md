# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="52056-101">Tipo de recurso windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="52056-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="52056-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52056-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52056-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="52056-103">Not yet documented</span></span>

<span data-ttu-id="52056-104">Herda de [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="52056-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52056-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52056-105">Properties</span></span>
|<span data-ttu-id="52056-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52056-106">Property</span></span>|<span data-ttu-id="52056-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="52056-107">Type</span></span>|<span data-ttu-id="52056-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="52056-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52056-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="52056-109">activeHoursStart</span></span>|<span data-ttu-id="52056-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="52056-110">TimeOfDay</span></span>|<span data-ttu-id="52056-111">Início das horas ativas</span><span class="sxs-lookup"><span data-stu-id="52056-111">Active Hours Start</span></span>|
|<span data-ttu-id="52056-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="52056-112">activeHoursEnd</span></span>|<span data-ttu-id="52056-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="52056-113">TimeOfDay</span></span>|<span data-ttu-id="52056-114">Final das horas ativas</span><span class="sxs-lookup"><span data-stu-id="52056-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="52056-115">Relações</span><span class="sxs-lookup"><span data-stu-id="52056-115">Relationships</span></span>
<span data-ttu-id="52056-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52056-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52056-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52056-117">JSON Representation</span></span>
<span data-ttu-id="52056-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52056-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



