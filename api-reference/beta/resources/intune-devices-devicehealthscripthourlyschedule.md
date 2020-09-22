---
title: tipo de recurso deviceHealthScriptHourlySchedule
description: Tipo de script de integridade do dispositivo agendamento por hora.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8365e4897a75df8c4247183aea37e1415ac893a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060332"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="27b93-103">tipo de recurso deviceHealthScriptHourlySchedule</span><span class="sxs-lookup"><span data-stu-id="27b93-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="27b93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27b93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27b93-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27b93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27b93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27b93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27b93-107">Tipo de script de integridade do dispositivo agendamento por hora.</span><span class="sxs-lookup"><span data-stu-id="27b93-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="27b93-108">Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="27b93-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27b93-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27b93-109">Properties</span></span>
|<span data-ttu-id="27b93-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27b93-110">Property</span></span>|<span data-ttu-id="27b93-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="27b93-111">Type</span></span>|<span data-ttu-id="27b93-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="27b93-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27b93-113">interval</span><span class="sxs-lookup"><span data-stu-id="27b93-113">interval</span></span>|<span data-ttu-id="27b93-114">Int32</span><span class="sxs-lookup"><span data-stu-id="27b93-114">Int32</span></span>|<span data-ttu-id="27b93-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="27b93-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="27b93-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="27b93-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="27b93-117">Relações</span><span class="sxs-lookup"><span data-stu-id="27b93-117">Relationships</span></span>
<span data-ttu-id="27b93-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27b93-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27b93-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27b93-119">JSON Representation</span></span>
<span data-ttu-id="27b93-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27b93-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```






