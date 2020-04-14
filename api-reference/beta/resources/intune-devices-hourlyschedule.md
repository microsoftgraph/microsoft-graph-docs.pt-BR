---
title: tipo de recurso hourlySchedule
description: Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2eae0d244eb78e006f74c127a81df1786bc9bd8f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470610"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="c8048-103">tipo de recurso hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="c8048-103">hourlySchedule resource type</span></span>

<span data-ttu-id="c8048-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8048-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8048-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8048-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8048-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8048-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8048-107">Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="c8048-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="c8048-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c8048-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8048-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8048-109">Properties</span></span>
|<span data-ttu-id="c8048-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8048-110">Property</span></span>|<span data-ttu-id="c8048-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8048-111">Type</span></span>|<span data-ttu-id="c8048-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8048-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8048-113">interval</span><span class="sxs-lookup"><span data-stu-id="c8048-113">interval</span></span>|<span data-ttu-id="c8048-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c8048-114">Int32</span></span>|<span data-ttu-id="c8048-115">Intervalo em número de horas</span><span class="sxs-lookup"><span data-stu-id="c8048-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8048-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c8048-116">Relationships</span></span>
<span data-ttu-id="c8048-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8048-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8048-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8048-118">JSON Representation</span></span>
<span data-ttu-id="c8048-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8048-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```



