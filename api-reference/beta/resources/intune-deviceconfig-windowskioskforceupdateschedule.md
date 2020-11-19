---
title: tipo de recurso windowsKioskForceUpdateSchedule
description: Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3dd2e5872a60884050cd7a32408288955e94f92
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276165"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="3692e-103">tipo de recurso windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="3692e-103">windowsKioskForceUpdateSchedule resource type</span></span>

<span data-ttu-id="3692e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3692e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3692e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3692e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3692e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3692e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3692e-107">Agendamento de atualização forçada do Windows 10 para dispositivos quiosque.</span><span class="sxs-lookup"><span data-stu-id="3692e-107">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="3692e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3692e-108">Properties</span></span>
|<span data-ttu-id="3692e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3692e-109">Property</span></span>|<span data-ttu-id="3692e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3692e-110">Type</span></span>|<span data-ttu-id="3692e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3692e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3692e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3692e-112">startDateTime</span></span>|<span data-ttu-id="3692e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3692e-113">DateTimeOffset</span></span>|<span data-ttu-id="3692e-114">A hora de início da reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="3692e-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="3692e-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="3692e-115">recurrence</span></span>|[<span data-ttu-id="3692e-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="3692e-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="3692e-117">Agenda de recorrência.</span><span class="sxs-lookup"><span data-stu-id="3692e-117">Recurrence schedule.</span></span> <span data-ttu-id="3692e-118">Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="3692e-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="3692e-119">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="3692e-119">dayofWeek</span></span>|[<span data-ttu-id="3692e-120">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="3692e-120">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="3692e-121">Dia da semana.</span><span class="sxs-lookup"><span data-stu-id="3692e-121">Day of week.</span></span> <span data-ttu-id="3692e-122">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="3692e-122">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3692e-123">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="3692e-123">dayofMonth</span></span>|<span data-ttu-id="3692e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3692e-124">Int32</span></span>|<span data-ttu-id="3692e-125">Dia do mês.</span><span class="sxs-lookup"><span data-stu-id="3692e-125">Day of month.</span></span> <span data-ttu-id="3692e-126">Valores válidos de 1 a 31</span><span class="sxs-lookup"><span data-stu-id="3692e-126">Valid values 1 to 31</span></span>|
|<span data-ttu-id="3692e-127">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="3692e-127">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="3692e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="3692e-128">Boolean</span></span>|<span data-ttu-id="3692e-129">Se true, executará a tarefa imediatamente se StartDatetime estiver no passado, senão, será executado na próxima recorrência.</span><span class="sxs-lookup"><span data-stu-id="3692e-129">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3692e-130">Relações</span><span class="sxs-lookup"><span data-stu-id="3692e-130">Relationships</span></span>
<span data-ttu-id="3692e-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3692e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3692e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3692e-132">JSON Representation</span></span>
<span data-ttu-id="3692e-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3692e-133">Here is a JSON representation of the resource.</span></span>
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




