---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
ms.openlocfilehash: 06e26bfb43691c8774e166a65b36d6ab872d44e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004916"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="9efe8-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="9efe8-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="9efe8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9efe8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9efe8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9efe8-105">Not yet documented</span></span>

<span data-ttu-id="9efe8-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="9efe8-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9efe8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9efe8-107">Properties</span></span>
|<span data-ttu-id="9efe8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9efe8-108">Property</span></span>|<span data-ttu-id="9efe8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9efe8-109">Type</span></span>|<span data-ttu-id="9efe8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9efe8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9efe8-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="9efe8-111">scheduledInstallDay</span></span>|[<span data-ttu-id="9efe8-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="9efe8-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="9efe8-113">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="9efe8-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="9efe8-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="9efe8-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="9efe8-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="9efe8-115">scheduledInstallTime</span></span>|<span data-ttu-id="9efe8-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9efe8-116">TimeOfDay</span></span>|<span data-ttu-id="9efe8-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="9efe8-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="9efe8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9efe8-118">Relationships</span></span>
<span data-ttu-id="9efe8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9efe8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9efe8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9efe8-120">JSON Representation</span></span>
<span data-ttu-id="9efe8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9efe8-121">Here is a JSON representation of the resource.</span></span>
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



