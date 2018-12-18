---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 4a8943fa0275d8b9e5a668be207c90304f22a327
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340912"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="647d5-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="647d5-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="647d5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="647d5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="647d5-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="647d5-105">Not yet documented</span></span>

<span data-ttu-id="647d5-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="647d5-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="647d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="647d5-107">Properties</span></span>
|<span data-ttu-id="647d5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="647d5-108">Property</span></span>|<span data-ttu-id="647d5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="647d5-109">Type</span></span>|<span data-ttu-id="647d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="647d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="647d5-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="647d5-111">scheduledInstallDay</span></span>|[<span data-ttu-id="647d5-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="647d5-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="647d5-113">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="647d5-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="647d5-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="647d5-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="647d5-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="647d5-115">scheduledInstallTime</span></span>|<span data-ttu-id="647d5-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="647d5-116">TimeOfDay</span></span>|<span data-ttu-id="647d5-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="647d5-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="647d5-118">Relações</span><span class="sxs-lookup"><span data-stu-id="647d5-118">Relationships</span></span>
<span data-ttu-id="647d5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="647d5-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="647d5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="647d5-120">JSON Representation</span></span>
<span data-ttu-id="647d5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="647d5-121">Here is a JSON representation of the resource.</span></span>
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



