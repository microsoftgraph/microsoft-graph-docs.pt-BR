---
title: tipo de recurso deviceHealthScriptHourlySchedule
description: Tipo de script de integridade do dispositivo agendamento por hora.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2276d95d09a1628b07d3b9bc87381b0d85d431f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176104"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="2cc69-103">tipo de recurso deviceHealthScriptHourlySchedule</span><span class="sxs-lookup"><span data-stu-id="2cc69-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="2cc69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cc69-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cc69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cc69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc69-107">Tipo de script de integridade do dispositivo agendamento por hora.</span><span class="sxs-lookup"><span data-stu-id="2cc69-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="2cc69-108">Herda de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="2cc69-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2cc69-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cc69-109">Properties</span></span>
|<span data-ttu-id="2cc69-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cc69-110">Property</span></span>|<span data-ttu-id="2cc69-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cc69-111">Type</span></span>|<span data-ttu-id="2cc69-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc69-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc69-113">interval</span><span class="sxs-lookup"><span data-stu-id="2cc69-113">interval</span></span>|<span data-ttu-id="2cc69-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2cc69-114">Int32</span></span>|<span data-ttu-id="2cc69-115">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="2cc69-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="2cc69-116">Valores válidos de 1 a 23 herdados de [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="2cc69-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc69-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2cc69-117">Relationships</span></span>
<span data-ttu-id="2cc69-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cc69-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc69-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cc69-119">JSON Representation</span></span>
<span data-ttu-id="2cc69-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cc69-120">Here is a JSON representation of the resource.</span></span>
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



