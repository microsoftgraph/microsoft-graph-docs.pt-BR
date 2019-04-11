---
title: tipo de recurso hourlySchedule
description: Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f86591326f2b4df8e887c657c05ad3d5021946e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778044"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="86182-103">tipo de recurso hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="86182-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="86182-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86182-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86182-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86182-106">Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="86182-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="86182-107">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="86182-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86182-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86182-108">Properties</span></span>
|<span data-ttu-id="86182-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86182-109">Property</span></span>|<span data-ttu-id="86182-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86182-110">Type</span></span>|<span data-ttu-id="86182-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86182-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86182-112">interval</span><span class="sxs-lookup"><span data-stu-id="86182-112">interval</span></span>|<span data-ttu-id="86182-113">Int32</span><span class="sxs-lookup"><span data-stu-id="86182-113">Int32</span></span>|<span data-ttu-id="86182-114">Intervalo em número de horas</span><span class="sxs-lookup"><span data-stu-id="86182-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="86182-115">Relações</span><span class="sxs-lookup"><span data-stu-id="86182-115">Relationships</span></span>
<span data-ttu-id="86182-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="86182-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86182-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86182-117">JSON Representation</span></span>
<span data-ttu-id="86182-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86182-118">Here is a JSON representation of the resource.</span></span>
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





