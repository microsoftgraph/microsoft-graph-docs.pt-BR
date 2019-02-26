---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de36e3777518cf7c79a7590c19147d014e2aee7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172503"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6b503-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="6b503-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="6b503-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b503-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b503-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b503-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b503-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6b503-106">Not yet documented</span></span>


<span data-ttu-id="6b503-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6b503-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b503-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b503-108">Properties</span></span>
|<span data-ttu-id="6b503-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b503-109">Property</span></span>|<span data-ttu-id="6b503-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b503-110">Type</span></span>|<span data-ttu-id="6b503-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b503-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b503-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6b503-112">scheduledInstallDay</span></span>|[<span data-ttu-id="6b503-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="6b503-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6b503-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="6b503-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="6b503-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6b503-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6b503-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6b503-116">scheduledInstallTime</span></span>|<span data-ttu-id="6b503-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6b503-117">TimeOfDay</span></span>|<span data-ttu-id="6b503-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="6b503-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b503-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6b503-119">Relationships</span></span>
<span data-ttu-id="6b503-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b503-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b503-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b503-121">JSON Representation</span></span>
<span data-ttu-id="6b503-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b503-122">Here is a JSON representation of the resource.</span></span>
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




