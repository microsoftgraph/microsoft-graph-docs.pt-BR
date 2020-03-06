---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ab68aa48d83e47e6cdbd3afc45ade10545b0590
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530317"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="f451e-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="f451e-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="f451e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f451e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f451e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f451e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f451e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f451e-106">Not yet documented</span></span>


<span data-ttu-id="f451e-107">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="f451e-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f451e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f451e-108">Properties</span></span>
|<span data-ttu-id="f451e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f451e-109">Property</span></span>|<span data-ttu-id="f451e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f451e-110">Type</span></span>|<span data-ttu-id="f451e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f451e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f451e-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="f451e-112">scheduledInstallDay</span></span>|[<span data-ttu-id="f451e-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="f451e-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="f451e-114">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="f451e-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="f451e-115">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f451e-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f451e-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="f451e-116">scheduledInstallTime</span></span>|<span data-ttu-id="f451e-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f451e-117">TimeOfDay</span></span>|<span data-ttu-id="f451e-118">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="f451e-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="f451e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f451e-119">Relationships</span></span>
<span data-ttu-id="f451e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f451e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f451e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f451e-121">JSON Representation</span></span>
<span data-ttu-id="f451e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f451e-122">Here is a JSON representation of the resource.</span></span>
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




