---
title: tipo de recurso deviceHealthScriptRunOnceSchedule
description: Script de integridade do dispositivo executado após a agenda.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4df6220bc95cd98e07a49073c3a7e5da6ab4096d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060269"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a><span data-ttu-id="69401-103">tipo de recurso deviceHealthScriptRunOnceSchedule</span><span class="sxs-lookup"><span data-stu-id="69401-103">deviceHealthScriptRunOnceSchedule resource type</span></span>

<span data-ttu-id="69401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69401-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69401-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69401-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69401-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69401-107">Script de integridade do dispositivo executado após a agenda.</span><span class="sxs-lookup"><span data-stu-id="69401-107">Device health script run once schedule.</span></span>


<span data-ttu-id="69401-108">Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="69401-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69401-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69401-109">Properties</span></span>
|<span data-ttu-id="69401-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69401-110">Property</span></span>|<span data-ttu-id="69401-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="69401-111">Type</span></span>|<span data-ttu-id="69401-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="69401-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69401-113">interval</span><span class="sxs-lookup"><span data-stu-id="69401-113">interval</span></span>|<span data-ttu-id="69401-114">Int32</span><span class="sxs-lookup"><span data-stu-id="69401-114">Int32</span></span>|<span data-ttu-id="69401-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="69401-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="69401-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="69401-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="69401-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="69401-117">useUtc</span></span>|<span data-ttu-id="69401-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="69401-118">Boolean</span></span>|<span data-ttu-id="69401-119">Indique se a hora é UTC ou horário local do cliente.</span><span class="sxs-lookup"><span data-stu-id="69401-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="69401-120">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="69401-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="69401-121">time</span><span class="sxs-lookup"><span data-stu-id="69401-121">time</span></span>|<span data-ttu-id="69401-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="69401-122">TimeOfDay</span></span>|<span data-ttu-id="69401-123">Em que tempo o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="69401-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="69401-124">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="69401-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="69401-125">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="69401-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="69401-126">data</span><span class="sxs-lookup"><span data-stu-id="69401-126">date</span></span>|<span data-ttu-id="69401-127">Data</span><span class="sxs-lookup"><span data-stu-id="69401-127">Date</span></span>|<span data-ttu-id="69401-128">A data em que o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="69401-128">The date the script is scheduled to run.</span></span> <span data-ttu-id="69401-129">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="69401-129">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69401-130">Relações</span><span class="sxs-lookup"><span data-stu-id="69401-130">Relationships</span></span>
<span data-ttu-id="69401-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69401-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69401-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69401-132">JSON Representation</span></span>
<span data-ttu-id="69401-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69401-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```






