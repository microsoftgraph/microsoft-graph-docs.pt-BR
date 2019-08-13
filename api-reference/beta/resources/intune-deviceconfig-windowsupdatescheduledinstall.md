---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93866da8e1dff5b53303dfd6cbd358fc0280ee30
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337682"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="8b181-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="8b181-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="8b181-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b181-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b181-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b181-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8b181-106">Not yet documented</span></span>


<span data-ttu-id="8b181-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8b181-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8b181-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b181-108">Properties</span></span>
|<span data-ttu-id="8b181-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b181-109">Property</span></span>|<span data-ttu-id="8b181-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b181-110">Type</span></span>|<span data-ttu-id="8b181-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b181-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b181-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="8b181-112">scheduledInstallDay</span></span>|[<span data-ttu-id="8b181-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8b181-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="8b181-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="8b181-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="8b181-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="8b181-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="8b181-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="8b181-116">scheduledInstallTime</span></span>|<span data-ttu-id="8b181-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8b181-117">TimeOfDay</span></span>|<span data-ttu-id="8b181-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="8b181-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b181-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8b181-119">Relationships</span></span>
<span data-ttu-id="8b181-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b181-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b181-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b181-121">JSON Representation</span></span>
<span data-ttu-id="8b181-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b181-122">Here is a JSON representation of the resource.</span></span>
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



