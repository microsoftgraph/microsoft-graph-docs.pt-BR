---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d392cf9f59a5af5999676d0d346dcc3b64252e66
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706944"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="3b597-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="3b597-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="3b597-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b597-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b597-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b597-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b597-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b597-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b597-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b597-107">Not yet documented</span></span>


<span data-ttu-id="3b597-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="3b597-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b597-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b597-109">Properties</span></span>
|<span data-ttu-id="3b597-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b597-110">Property</span></span>|<span data-ttu-id="3b597-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b597-111">Type</span></span>|<span data-ttu-id="3b597-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b597-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b597-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="3b597-113">scheduledInstallDay</span></span>|[<span data-ttu-id="3b597-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="3b597-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="3b597-115">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="3b597-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="3b597-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="3b597-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="3b597-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="3b597-117">scheduledInstallTime</span></span>|<span data-ttu-id="3b597-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3b597-118">TimeOfDay</span></span>|<span data-ttu-id="3b597-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="3b597-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b597-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3b597-120">Relationships</span></span>
<span data-ttu-id="3b597-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b597-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b597-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b597-122">JSON Representation</span></span>
<span data-ttu-id="3b597-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b597-123">Here is a JSON representation of the resource.</span></span>
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





