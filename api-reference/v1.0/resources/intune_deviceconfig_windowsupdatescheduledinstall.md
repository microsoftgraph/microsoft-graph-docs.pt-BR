# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="8e614-101">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="8e614-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="8e614-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e614-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e614-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8e614-103">Not yet documented</span></span>

<span data-ttu-id="8e614-104">Herda de [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8e614-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e614-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e614-105">Properties</span></span>
|<span data-ttu-id="8e614-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e614-106">Property</span></span>|<span data-ttu-id="8e614-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e614-107">Type</span></span>|<span data-ttu-id="8e614-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e614-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e614-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="8e614-109">scheduledInstallDay</span></span>|[<span data-ttu-id="8e614-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8e614-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="8e614-111">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="8e614-111">Scheduled Install Day in week.</span></span> <span data-ttu-id="8e614-112">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="8e614-112">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8e614-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="8e614-113">scheduledInstallTime</span></span>|<span data-ttu-id="8e614-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8e614-114">TimeOfDay</span></span>|<span data-ttu-id="8e614-115">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="8e614-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e614-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8e614-116">Relationships</span></span>
<span data-ttu-id="8e614-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e614-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e614-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e614-118">JSON Representation</span></span>
<span data-ttu-id="8e614-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e614-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



