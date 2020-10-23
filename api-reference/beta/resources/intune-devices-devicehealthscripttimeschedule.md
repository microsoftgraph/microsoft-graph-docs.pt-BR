---
title: tipo de recurso deviceHealthScriptTimeSchedule
description: Tipo base de agendamento do tempo de script de integridade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29f6e8b413e008b09c9314f0bd1c505b3d39eab6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694981"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a><span data-ttu-id="77c33-103">tipo de recurso deviceHealthScriptTimeSchedule</span><span class="sxs-lookup"><span data-stu-id="77c33-103">deviceHealthScriptTimeSchedule resource type</span></span>

<span data-ttu-id="77c33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77c33-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77c33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77c33-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77c33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77c33-107">Tipo base de agendamento do tempo de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77c33-107">Base type of Device health script time schedule.</span></span>


<span data-ttu-id="77c33-108">Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="77c33-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77c33-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77c33-109">Properties</span></span>
|<span data-ttu-id="77c33-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77c33-110">Property</span></span>|<span data-ttu-id="77c33-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="77c33-111">Type</span></span>|<span data-ttu-id="77c33-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="77c33-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77c33-113">interval</span><span class="sxs-lookup"><span data-stu-id="77c33-113">interval</span></span>|<span data-ttu-id="77c33-114">Int32</span><span class="sxs-lookup"><span data-stu-id="77c33-114">Int32</span></span>|<span data-ttu-id="77c33-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="77c33-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="77c33-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="77c33-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="77c33-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="77c33-117">useUtc</span></span>|<span data-ttu-id="77c33-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="77c33-118">Boolean</span></span>|<span data-ttu-id="77c33-119">Indique se a hora é UTC ou horário local do cliente.</span><span class="sxs-lookup"><span data-stu-id="77c33-119">Indicate if the time is Utc or client local time.</span></span>|
|<span data-ttu-id="77c33-120">hora</span><span class="sxs-lookup"><span data-stu-id="77c33-120">time</span></span>|<span data-ttu-id="77c33-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="77c33-121">TimeOfDay</span></span>|<span data-ttu-id="77c33-122">Em que tempo o script está agendado para ser executado.</span><span class="sxs-lookup"><span data-stu-id="77c33-122">At what time the script is scheduled to run.</span></span> <span data-ttu-id="77c33-123">Essa coleção pode conter um máximo de 20 elementos.</span><span class="sxs-lookup"><span data-stu-id="77c33-123">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77c33-124">Relações</span><span class="sxs-lookup"><span data-stu-id="77c33-124">Relationships</span></span>
<span data-ttu-id="77c33-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77c33-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77c33-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77c33-126">JSON Representation</span></span>
<span data-ttu-id="77c33-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77c33-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptTimeSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptTimeSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```





