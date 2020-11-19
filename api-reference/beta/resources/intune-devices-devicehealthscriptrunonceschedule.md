---
title: tipo de recurso deviceHealthScriptRunOnceSchedule
description: Script de integridade do dispositivo executado após a agenda.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 230d9592b66f85457b20343a48d8024a9b4afe87
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299419"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a><span data-ttu-id="aaf31-103">tipo de recurso deviceHealthScriptRunOnceSchedule</span><span class="sxs-lookup"><span data-stu-id="aaf31-103">deviceHealthScriptRunOnceSchedule resource type</span></span>

<span data-ttu-id="aaf31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaf31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaf31-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aaf31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf31-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aaf31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf31-107">Script de integridade do dispositivo executado após a agenda.</span><span class="sxs-lookup"><span data-stu-id="aaf31-107">Device health script run once schedule.</span></span>


<span data-ttu-id="aaf31-108">Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="aaf31-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aaf31-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aaf31-109">Properties</span></span>
|<span data-ttu-id="aaf31-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaf31-110">Property</span></span>|<span data-ttu-id="aaf31-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaf31-111">Type</span></span>|<span data-ttu-id="aaf31-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaf31-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf31-113">interval</span><span class="sxs-lookup"><span data-stu-id="aaf31-113">interval</span></span>|<span data-ttu-id="aaf31-114">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf31-114">Int32</span></span>|<span data-ttu-id="aaf31-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="aaf31-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="aaf31-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="aaf31-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="aaf31-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="aaf31-117">useUtc</span></span>|<span data-ttu-id="aaf31-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="aaf31-118">Boolean</span></span>|<span data-ttu-id="aaf31-119">Indique se a hora é UTC ou horário local do cliente.</span><span class="sxs-lookup"><span data-stu-id="aaf31-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="aaf31-120">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="aaf31-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="aaf31-121">hora</span><span class="sxs-lookup"><span data-stu-id="aaf31-121">time</span></span>|<span data-ttu-id="aaf31-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="aaf31-122">TimeOfDay</span></span>|<span data-ttu-id="aaf31-123">Em que tempo o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="aaf31-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="aaf31-124">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="aaf31-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="aaf31-125">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="aaf31-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="aaf31-126">data</span><span class="sxs-lookup"><span data-stu-id="aaf31-126">date</span></span>|<span data-ttu-id="aaf31-127">Data</span><span class="sxs-lookup"><span data-stu-id="aaf31-127">Date</span></span>|<span data-ttu-id="aaf31-128">A data em que o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="aaf31-128">The date the script is scheduled to run.</span></span> <span data-ttu-id="aaf31-129">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="aaf31-129">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaf31-130">Relações</span><span class="sxs-lookup"><span data-stu-id="aaf31-130">Relationships</span></span>
<span data-ttu-id="aaf31-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aaf31-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaf31-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aaf31-132">JSON Representation</span></span>
<span data-ttu-id="aaf31-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aaf31-133">Here is a JSON representation of the resource.</span></span>
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




