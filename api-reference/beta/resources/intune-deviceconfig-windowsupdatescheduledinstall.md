---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd3a1aafe751bd5db334387cc3872c68e6de6637
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797918"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="bf492-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="bf492-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="bf492-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf492-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf492-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf492-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf492-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bf492-106">Not yet documented</span></span>


<span data-ttu-id="bf492-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="bf492-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf492-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf492-108">Properties</span></span>
|<span data-ttu-id="bf492-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf492-109">Property</span></span>|<span data-ttu-id="bf492-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf492-110">Type</span></span>|<span data-ttu-id="bf492-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf492-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf492-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="bf492-112">scheduledInstallDay</span></span>|[<span data-ttu-id="bf492-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="bf492-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="bf492-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="bf492-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="bf492-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="bf492-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="bf492-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="bf492-116">scheduledInstallTime</span></span>|<span data-ttu-id="bf492-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bf492-117">TimeOfDay</span></span>|<span data-ttu-id="bf492-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="bf492-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf492-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bf492-119">Relationships</span></span>
<span data-ttu-id="bf492-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bf492-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf492-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf492-121">JSON Representation</span></span>
<span data-ttu-id="bf492-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf492-122">Here is a JSON representation of the resource.</span></span>
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





