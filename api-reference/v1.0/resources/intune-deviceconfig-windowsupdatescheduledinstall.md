---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22c1c6e2ba205c705baabc6bc7643848f7f12686
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759949"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="a827e-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="a827e-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="a827e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a827e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a827e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a827e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a827e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a827e-106">Not yet documented</span></span>


<span data-ttu-id="a827e-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="a827e-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a827e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a827e-108">Properties</span></span>
|<span data-ttu-id="a827e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a827e-109">Property</span></span>|<span data-ttu-id="a827e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a827e-110">Type</span></span>|<span data-ttu-id="a827e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a827e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a827e-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="a827e-112">scheduledInstallDay</span></span>|[<span data-ttu-id="a827e-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="a827e-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="a827e-114">Dia de instalação agendado na semana.</span><span class="sxs-lookup"><span data-stu-id="a827e-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="a827e-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="a827e-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a827e-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="a827e-116">scheduledInstallTime</span></span>|<span data-ttu-id="a827e-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a827e-117">TimeOfDay</span></span>|<span data-ttu-id="a827e-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="a827e-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="a827e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a827e-119">Relationships</span></span>
<span data-ttu-id="a827e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a827e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a827e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a827e-121">JSON Representation</span></span>
<span data-ttu-id="a827e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a827e-122">Here is a JSON representation of the resource.</span></span>
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




