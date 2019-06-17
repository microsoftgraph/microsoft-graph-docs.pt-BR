---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0af2edc973e18c6afde50d1fdc5d93c5db196bf3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978693"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="47718-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="47718-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="47718-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47718-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47718-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47718-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47718-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="47718-106">Not yet documented</span></span>


<span data-ttu-id="47718-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="47718-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47718-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47718-108">Properties</span></span>
|<span data-ttu-id="47718-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47718-109">Property</span></span>|<span data-ttu-id="47718-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="47718-110">Type</span></span>|<span data-ttu-id="47718-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47718-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47718-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="47718-112">scheduledInstallDay</span></span>|[<span data-ttu-id="47718-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="47718-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="47718-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="47718-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="47718-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="47718-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="47718-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="47718-116">scheduledInstallTime</span></span>|<span data-ttu-id="47718-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="47718-117">TimeOfDay</span></span>|<span data-ttu-id="47718-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="47718-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="47718-119">Relações</span><span class="sxs-lookup"><span data-stu-id="47718-119">Relationships</span></span>
<span data-ttu-id="47718-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47718-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47718-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47718-121">JSON Representation</span></span>
<span data-ttu-id="47718-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47718-122">Here is a JSON representation of the resource.</span></span>
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





