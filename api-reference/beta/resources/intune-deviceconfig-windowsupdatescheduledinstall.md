---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 270df73ef5db5cde3784adb797475b9232591de6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943617"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="77663-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="77663-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="77663-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77663-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77663-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77663-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77663-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="77663-106">Not yet documented</span></span>


<span data-ttu-id="77663-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="77663-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77663-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77663-108">Properties</span></span>
|<span data-ttu-id="77663-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77663-109">Property</span></span>|<span data-ttu-id="77663-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="77663-110">Type</span></span>|<span data-ttu-id="77663-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77663-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77663-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="77663-112">scheduledInstallDay</span></span>|[<span data-ttu-id="77663-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="77663-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="77663-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="77663-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="77663-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="77663-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="77663-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="77663-116">scheduledInstallTime</span></span>|<span data-ttu-id="77663-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="77663-117">TimeOfDay</span></span>|<span data-ttu-id="77663-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="77663-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="77663-119">Relações</span><span class="sxs-lookup"><span data-stu-id="77663-119">Relationships</span></span>
<span data-ttu-id="77663-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77663-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77663-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77663-121">JSON Representation</span></span>
<span data-ttu-id="77663-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77663-122">Here is a JSON representation of the resource.</span></span>
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




