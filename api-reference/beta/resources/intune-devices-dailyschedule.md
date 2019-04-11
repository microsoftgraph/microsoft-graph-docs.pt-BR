---
title: tipo de recurso dailySchedule
description: Agenda de execução diária de um script de gerenciamento de dispositivo recorrente.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd2b226255f433b4f82d042b6389830143515033
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788069"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="41b1c-103">tipo de recurso dailySchedule</span><span class="sxs-lookup"><span data-stu-id="41b1c-103">dailySchedule resource type</span></span>

> <span data-ttu-id="41b1c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41b1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41b1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41b1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41b1c-106">Agenda de execução diária de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="41b1c-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="41b1c-107">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="41b1c-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41b1c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41b1c-108">Properties</span></span>
|<span data-ttu-id="41b1c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41b1c-109">Property</span></span>|<span data-ttu-id="41b1c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41b1c-110">Type</span></span>|<span data-ttu-id="41b1c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41b1c-112">interval</span><span class="sxs-lookup"><span data-stu-id="41b1c-112">interval</span></span>|<span data-ttu-id="41b1c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="41b1c-113">Int32</span></span>|<span data-ttu-id="41b1c-114">Intervalo em número de dias</span><span class="sxs-lookup"><span data-stu-id="41b1c-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="41b1c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="41b1c-115">Relationships</span></span>
<span data-ttu-id="41b1c-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="41b1c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41b1c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41b1c-117">JSON Representation</span></span>
<span data-ttu-id="41b1c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41b1c-118">Here is a JSON representation of the resource.</span></span>
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





