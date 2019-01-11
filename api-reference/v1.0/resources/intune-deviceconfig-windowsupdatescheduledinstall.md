---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19e0ced371108103398e26c6067f4ce3b3ab67e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806402"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="765f8-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="765f8-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="765f8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="765f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="765f8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="765f8-105">Not yet documented</span></span>

<span data-ttu-id="765f8-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="765f8-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="765f8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="765f8-107">Properties</span></span>
|<span data-ttu-id="765f8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="765f8-108">Property</span></span>|<span data-ttu-id="765f8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="765f8-109">Type</span></span>|<span data-ttu-id="765f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="765f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="765f8-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="765f8-111">scheduledInstallDay</span></span>|[<span data-ttu-id="765f8-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="765f8-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="765f8-113">Agendada instalar o dia na semana.</span><span class="sxs-lookup"><span data-stu-id="765f8-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="765f8-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="765f8-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="765f8-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="765f8-115">scheduledInstallTime</span></span>|<span data-ttu-id="765f8-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="765f8-116">TimeOfDay</span></span>|<span data-ttu-id="765f8-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="765f8-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="765f8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="765f8-118">Relationships</span></span>
<span data-ttu-id="765f8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="765f8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="765f8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="765f8-120">JSON Representation</span></span>
<span data-ttu-id="765f8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="765f8-121">Here is a JSON representation of the resource.</span></span>
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



