---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca4c658c9fa9837deb56868a84ff0bddefeb6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272413"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="a524c-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="a524c-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="a524c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a524c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a524c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a524c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a524c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a524c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a524c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a524c-107">Not yet documented</span></span>


<span data-ttu-id="a524c-108">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a524c-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a524c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a524c-109">Properties</span></span>
|<span data-ttu-id="a524c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a524c-110">Property</span></span>|<span data-ttu-id="a524c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a524c-111">Type</span></span>|<span data-ttu-id="a524c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a524c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a524c-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="a524c-113">scheduledInstallDay</span></span>|[<span data-ttu-id="a524c-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="a524c-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="a524c-115">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="a524c-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="a524c-116">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="a524c-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="a524c-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="a524c-117">scheduledInstallTime</span></span>|<span data-ttu-id="a524c-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a524c-118">TimeOfDay</span></span>|<span data-ttu-id="a524c-119">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="a524c-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="a524c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a524c-120">Relationships</span></span>
<span data-ttu-id="a524c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a524c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a524c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a524c-122">JSON Representation</span></span>
<span data-ttu-id="a524c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a524c-123">Here is a JSON representation of the resource.</span></span>
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




