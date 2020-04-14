---
title: tipo de recurso dailySchedule
description: Agenda de execução diária de um script de gerenciamento de dispositivo recorrente.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b921b13fd87d3a500ca543ca6601a9ad368456ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464997"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="8ffc2-103">tipo de recurso dailySchedule</span><span class="sxs-lookup"><span data-stu-id="8ffc2-103">dailySchedule resource type</span></span>

<span data-ttu-id="8ffc2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ffc2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ffc2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ffc2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ffc2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ffc2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ffc2-107">Agenda de execução diária de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="8ffc2-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="8ffc2-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="8ffc2-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ffc2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ffc2-109">Properties</span></span>
|<span data-ttu-id="8ffc2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ffc2-110">Property</span></span>|<span data-ttu-id="8ffc2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ffc2-111">Type</span></span>|<span data-ttu-id="8ffc2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ffc2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ffc2-113">interval</span><span class="sxs-lookup"><span data-stu-id="8ffc2-113">interval</span></span>|<span data-ttu-id="8ffc2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8ffc2-114">Int32</span></span>|<span data-ttu-id="8ffc2-115">Intervalo em número de dias</span><span class="sxs-lookup"><span data-stu-id="8ffc2-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ffc2-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8ffc2-116">Relationships</span></span>
<span data-ttu-id="8ffc2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ffc2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ffc2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ffc2-118">JSON Representation</span></span>
<span data-ttu-id="8ffc2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ffc2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```



