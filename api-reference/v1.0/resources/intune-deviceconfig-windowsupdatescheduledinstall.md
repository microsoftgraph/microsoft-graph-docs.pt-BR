---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fd5958e5b8e853f07c715cd1ecf8c03a9a49a15
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357133"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="01845-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="01845-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="01845-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01845-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01845-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01845-105">Not yet documented</span></span>


<span data-ttu-id="01845-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="01845-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="01845-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01845-107">Properties</span></span>
|<span data-ttu-id="01845-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01845-108">Property</span></span>|<span data-ttu-id="01845-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="01845-109">Type</span></span>|<span data-ttu-id="01845-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="01845-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01845-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="01845-111">scheduledInstallDay</span></span>|[<span data-ttu-id="01845-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="01845-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="01845-113">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="01845-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="01845-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="01845-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="01845-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="01845-115">scheduledInstallTime</span></span>|<span data-ttu-id="01845-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="01845-116">TimeOfDay</span></span>|<span data-ttu-id="01845-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="01845-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="01845-118">Relações</span><span class="sxs-lookup"><span data-stu-id="01845-118">Relationships</span></span>
<span data-ttu-id="01845-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01845-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01845-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01845-120">JSON Representation</span></span>
<span data-ttu-id="01845-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01845-121">Here is a JSON representation of the resource.</span></span>
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




