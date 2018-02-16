# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="089cf-101">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="089cf-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="089cf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="089cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="089cf-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="089cf-103">Not yet documented</span></span>

<span data-ttu-id="089cf-104">Herda de [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="089cf-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="089cf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="089cf-105">Properties</span></span>
|<span data-ttu-id="089cf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="089cf-106">Property</span></span>|<span data-ttu-id="089cf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="089cf-107">Type</span></span>|<span data-ttu-id="089cf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="089cf-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089cf-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="089cf-109">scheduledInstallDay</span></span>|<span data-ttu-id="089cf-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="089cf-110">String</span></span>|<span data-ttu-id="089cf-111">Dia da semana para instalação agendada Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="089cf-111">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="089cf-112">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="089cf-112">scheduledInstallTime</span></span>|<span data-ttu-id="089cf-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="089cf-113">TimeOfDay</span></span>|<span data-ttu-id="089cf-114">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="089cf-114">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="089cf-115">Relações</span><span class="sxs-lookup"><span data-stu-id="089cf-115">Relationships</span></span>
<span data-ttu-id="089cf-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="089cf-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="089cf-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="089cf-117">JSON Representation</span></span>
<span data-ttu-id="089cf-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="089cf-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



