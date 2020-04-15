---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2b9173207c52029d4d65faafa2d6c8607423fe8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451359"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="5d59a-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="5d59a-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="5d59a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d59a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d59a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d59a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d59a-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5d59a-106">Not yet documented</span></span>


<span data-ttu-id="5d59a-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="5d59a-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d59a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d59a-108">Properties</span></span>
|<span data-ttu-id="5d59a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d59a-109">Property</span></span>|<span data-ttu-id="5d59a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d59a-110">Type</span></span>|<span data-ttu-id="5d59a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d59a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d59a-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="5d59a-112">scheduledInstallDay</span></span>|[<span data-ttu-id="5d59a-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="5d59a-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="5d59a-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="5d59a-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="5d59a-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="5d59a-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5d59a-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="5d59a-116">scheduledInstallTime</span></span>|<span data-ttu-id="5d59a-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5d59a-117">TimeOfDay</span></span>|<span data-ttu-id="5d59a-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="5d59a-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d59a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5d59a-119">Relationships</span></span>
<span data-ttu-id="5d59a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d59a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d59a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d59a-121">JSON Representation</span></span>
<span data-ttu-id="5d59a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d59a-122">Here is a JSON representation of the resource.</span></span>
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







