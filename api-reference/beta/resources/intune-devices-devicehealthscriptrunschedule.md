---
title: tipo de recurso deviceHealthScriptRunSchedule
description: Tipo base de agendamento de execução de script de integridade do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 813512f607b6b0bd4eaf633c41ccd5a28554936e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299377"
---
# <a name="devicehealthscriptrunschedule-resource-type"></a><span data-ttu-id="54916-103">tipo de recurso deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="54916-103">deviceHealthScriptRunSchedule resource type</span></span>

<span data-ttu-id="54916-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54916-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54916-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54916-107">Tipo base de agendamento de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54916-107">Base type of Device health script run schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="54916-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54916-108">Properties</span></span>
|<span data-ttu-id="54916-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54916-109">Property</span></span>|<span data-ttu-id="54916-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="54916-110">Type</span></span>|<span data-ttu-id="54916-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="54916-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54916-112">interval</span><span class="sxs-lookup"><span data-stu-id="54916-112">interval</span></span>|<span data-ttu-id="54916-113">Int32</span><span class="sxs-lookup"><span data-stu-id="54916-113">Int32</span></span>|<span data-ttu-id="54916-114">O valor x de cada x horas para agendamento por hora, a cada x dias para agenda diária, a cada x semanas para agenda semanal, a cada x meses para agenda mensal.</span><span class="sxs-lookup"><span data-stu-id="54916-114">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="54916-115">Valores válidos de 1 a 23</span><span class="sxs-lookup"><span data-stu-id="54916-115">Valid values 1 to 23</span></span>|

## <a name="relationships"></a><span data-ttu-id="54916-116">Relações</span><span class="sxs-lookup"><span data-stu-id="54916-116">Relationships</span></span>
<span data-ttu-id="54916-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54916-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54916-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54916-118">JSON Representation</span></span>
<span data-ttu-id="54916-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54916-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": 1024
}
```




