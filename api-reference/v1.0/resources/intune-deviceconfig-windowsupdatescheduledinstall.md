---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264313"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="07909-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="07909-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="07909-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07909-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07909-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07909-105">Not yet documented</span></span>


<span data-ttu-id="07909-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="07909-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07909-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07909-107">Properties</span></span>
|<span data-ttu-id="07909-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07909-108">Property</span></span>|<span data-ttu-id="07909-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="07909-109">Type</span></span>|<span data-ttu-id="07909-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07909-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07909-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="07909-111">scheduledInstallDay</span></span>|[<span data-ttu-id="07909-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="07909-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="07909-113">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="07909-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="07909-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="07909-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="07909-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="07909-115">scheduledInstallTime</span></span>|<span data-ttu-id="07909-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="07909-116">TimeOfDay</span></span>|<span data-ttu-id="07909-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="07909-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="07909-118">Relações</span><span class="sxs-lookup"><span data-stu-id="07909-118">Relationships</span></span>
<span data-ttu-id="07909-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07909-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07909-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07909-120">JSON Representation</span></span>
<span data-ttu-id="07909-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07909-121">Here is a JSON representation of the resource.</span></span>
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



