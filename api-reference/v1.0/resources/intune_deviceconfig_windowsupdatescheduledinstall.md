# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="a0e7a-101">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="a0e7a-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="a0e7a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e7a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0e7a-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0e7a-103">Not yet documented</span></span>

<span data-ttu-id="a0e7a-104">Herda de [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a0e7a-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0e7a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0e7a-105">Properties</span></span>
|<span data-ttu-id="a0e7a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0e7a-106">Property</span></span>|<span data-ttu-id="a0e7a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e7a-107">Type</span></span>|<span data-ttu-id="a0e7a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0e7a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e7a-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="a0e7a-109">scheduledInstallDay</span></span>|[<span data-ttu-id="a0e7a-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="a0e7a-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="a0e7a-p101">Dia da semana agendado para instalação. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="a0e7a-p101">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a0e7a-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="a0e7a-113">scheduledInstallTime</span></span>|<span data-ttu-id="a0e7a-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0e7a-114">TimeOfDay</span></span>|<span data-ttu-id="a0e7a-115">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="a0e7a-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e7a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a0e7a-116">Relationships</span></span>
<span data-ttu-id="a0e7a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0e7a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0e7a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0e7a-118">JSON Representation</span></span>
<span data-ttu-id="a0e7a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0e7a-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```








