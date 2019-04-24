---
title: Tipo de recurso windowsUpdateScheduledInstall
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503573"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="95f6d-103">Tipo de recurso windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="95f6d-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="95f6d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95f6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f6d-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95f6d-105">Not yet documented</span></span>


<span data-ttu-id="95f6d-106">Herda de [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="95f6d-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95f6d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95f6d-107">Properties</span></span>
|<span data-ttu-id="95f6d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95f6d-108">Property</span></span>|<span data-ttu-id="95f6d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="95f6d-109">Type</span></span>|<span data-ttu-id="95f6d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95f6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95f6d-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="95f6d-111">scheduledInstallDay</span></span>|[<span data-ttu-id="95f6d-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="95f6d-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="95f6d-113">Dia da instalação agendada da semana.</span><span class="sxs-lookup"><span data-stu-id="95f6d-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="95f6d-114">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="95f6d-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="95f6d-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="95f6d-115">scheduledInstallTime</span></span>|<span data-ttu-id="95f6d-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95f6d-116">TimeOfDay</span></span>|<span data-ttu-id="95f6d-117">Horário de instalação agendado durante o dia</span><span class="sxs-lookup"><span data-stu-id="95f6d-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="95f6d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="95f6d-118">Relationships</span></span>
<span data-ttu-id="95f6d-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="95f6d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95f6d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95f6d-120">JSON Representation</span></span>
<span data-ttu-id="95f6d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95f6d-121">Here is a JSON representation of the resource.</span></span>
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



