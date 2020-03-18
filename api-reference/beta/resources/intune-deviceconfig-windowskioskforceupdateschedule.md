---
title: tipo de recurso windowsKioskForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c1b9f1b82bc5edcbe1bdc7d1521ec669de5f6af
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786388"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="afd37-103">tipo de recurso windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="afd37-103">windowsKioskForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="afd37-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afd37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afd37-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afd37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afd37-106">Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.</span><span class="sxs-lookup"><span data-stu-id="afd37-106">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="afd37-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afd37-107">Properties</span></span>
|<span data-ttu-id="afd37-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afd37-108">Property</span></span>|<span data-ttu-id="afd37-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="afd37-109">Type</span></span>|<span data-ttu-id="afd37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="afd37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afd37-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="afd37-111">startDateTime</span></span>|<span data-ttu-id="afd37-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afd37-112">DateTimeOffset</span></span>|<span data-ttu-id="afd37-113">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="afd37-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="afd37-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="afd37-114">recurrence</span></span>|[<span data-ttu-id="afd37-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="afd37-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="afd37-116">Agenda de recorrência.</span><span class="sxs-lookup"><span data-stu-id="afd37-116">Recurrence schedule.</span></span> <span data-ttu-id="afd37-117">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="afd37-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="afd37-118">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="afd37-118">dayofWeek</span></span>|[<span data-ttu-id="afd37-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="afd37-119">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="afd37-120">Dia da semana.</span><span class="sxs-lookup"><span data-stu-id="afd37-120">Day of week.</span></span> <span data-ttu-id="afd37-121">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="afd37-121">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="afd37-122">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="afd37-122">dayofMonth</span></span>|<span data-ttu-id="afd37-123">Int32</span><span class="sxs-lookup"><span data-stu-id="afd37-123">Int32</span></span>|<span data-ttu-id="afd37-124">Dia do mês.</span><span class="sxs-lookup"><span data-stu-id="afd37-124">Day of month.</span></span> <span data-ttu-id="afd37-125">Valores válidos de 1 a 31</span><span class="sxs-lookup"><span data-stu-id="afd37-125">Valid values 1 to 31</span></span>|
|<span data-ttu-id="afd37-126">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="afd37-126">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="afd37-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="afd37-127">Boolean</span></span>|<span data-ttu-id="afd37-128">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="afd37-128">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afd37-129">Relações</span><span class="sxs-lookup"><span data-stu-id="afd37-129">Relationships</span></span>
<span data-ttu-id="afd37-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afd37-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afd37-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afd37-131">JSON Representation</span></span>
<span data-ttu-id="afd37-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afd37-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```



