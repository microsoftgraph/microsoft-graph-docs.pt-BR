---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ceb6330bddf03b230dca644217c70bf1e3bba5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441097"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="9faa2-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="9faa2-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="9faa2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9faa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9faa2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9faa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9faa2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9faa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9faa2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9faa2-107">Not yet documented</span></span>


<span data-ttu-id="9faa2-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="9faa2-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9faa2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9faa2-109">Properties</span></span>
|<span data-ttu-id="9faa2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9faa2-110">Property</span></span>|<span data-ttu-id="9faa2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9faa2-111">Type</span></span>|<span data-ttu-id="9faa2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9faa2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9faa2-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="9faa2-113">scheduledInstallDay</span></span>|[<span data-ttu-id="9faa2-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="9faa2-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="9faa2-115">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="9faa2-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="9faa2-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="9faa2-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="9faa2-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="9faa2-117">scheduledInstallTime</span></span>|<span data-ttu-id="9faa2-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9faa2-118">TimeOfDay</span></span>|<span data-ttu-id="9faa2-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="9faa2-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="9faa2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="9faa2-120">Relationships</span></span>
<span data-ttu-id="9faa2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9faa2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9faa2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9faa2-122">JSON Representation</span></span>
<span data-ttu-id="9faa2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9faa2-123">Here is a JSON representation of the resource.</span></span>
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



