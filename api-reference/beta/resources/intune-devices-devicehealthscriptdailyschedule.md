---
title: tipo de recurso deviceHealthScriptDailySchedule
description: Agendamento diário do script de integridade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 75413f45b8e6401e3d789e5f235a17ad8bd94f38
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176105"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a><span data-ttu-id="38f18-103">tipo de recurso deviceHealthScriptDailySchedule</span><span class="sxs-lookup"><span data-stu-id="38f18-103">deviceHealthScriptDailySchedule resource type</span></span>

<span data-ttu-id="38f18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38f18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38f18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38f18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38f18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38f18-107">Agendamento diário do script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38f18-107">Device health script daily schedule.</span></span>


<span data-ttu-id="38f18-108">Herda de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="38f18-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38f18-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38f18-109">Properties</span></span>
|<span data-ttu-id="38f18-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38f18-110">Property</span></span>|<span data-ttu-id="38f18-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="38f18-111">Type</span></span>|<span data-ttu-id="38f18-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f18-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38f18-113">interval</span><span class="sxs-lookup"><span data-stu-id="38f18-113">interval</span></span>|<span data-ttu-id="38f18-114">Int32</span><span class="sxs-lookup"><span data-stu-id="38f18-114">Int32</span></span>|<span data-ttu-id="38f18-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="38f18-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="38f18-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="38f18-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="38f18-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="38f18-117">useUtc</span></span>|<span data-ttu-id="38f18-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="38f18-118">Boolean</span></span>|<span data-ttu-id="38f18-119">Indique se a hora é UTC ou horário local do cliente.</span><span class="sxs-lookup"><span data-stu-id="38f18-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="38f18-120">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="38f18-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="38f18-121">time</span><span class="sxs-lookup"><span data-stu-id="38f18-121">time</span></span>|<span data-ttu-id="38f18-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="38f18-122">TimeOfDay</span></span>|<span data-ttu-id="38f18-123">Em que tempo o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="38f18-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="38f18-124">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="38f18-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="38f18-125">Herdado de [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="38f18-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="38f18-126">Relações</span><span class="sxs-lookup"><span data-stu-id="38f18-126">Relationships</span></span>
<span data-ttu-id="38f18-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38f18-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38f18-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38f18-128">JSON Representation</span></span>
<span data-ttu-id="38f18-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38f18-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDailySchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```



