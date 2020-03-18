---
title: tipo de recurso customUpdateTimeWindow
description: Janela de tempo de atualização personalizada
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f56cf571b24c2bcee52e82100f5c087772c336e5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795642"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="12b2b-103">tipo de recurso customUpdateTimeWindow</span><span class="sxs-lookup"><span data-stu-id="12b2b-103">customUpdateTimeWindow resource type</span></span>

> <span data-ttu-id="12b2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12b2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12b2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12b2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12b2b-106">Janela de tempo de atualização personalizada</span><span class="sxs-lookup"><span data-stu-id="12b2b-106">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="12b2b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12b2b-107">Properties</span></span>
|<span data-ttu-id="12b2b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12b2b-108">Property</span></span>|<span data-ttu-id="12b2b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12b2b-109">Type</span></span>|<span data-ttu-id="12b2b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12b2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b2b-111">startDay</span><span class="sxs-lookup"><span data-stu-id="12b2b-111">startDay</span></span>|[<span data-ttu-id="12b2b-112">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="12b2b-112">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="12b2b-113">Dia inicial da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="12b2b-113">Start day of the time window.</span></span> <span data-ttu-id="12b2b-114">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="12b2b-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="12b2b-115">endDay</span><span class="sxs-lookup"><span data-stu-id="12b2b-115">endDay</span></span>|[<span data-ttu-id="12b2b-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="12b2b-116">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="12b2b-117">Dia de término da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="12b2b-117">End day of the time window.</span></span> <span data-ttu-id="12b2b-118">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="12b2b-118">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="12b2b-119">startTime</span><span class="sxs-lookup"><span data-stu-id="12b2b-119">startTime</span></span>|<span data-ttu-id="12b2b-120">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12b2b-120">TimeOfDay</span></span>|<span data-ttu-id="12b2b-121">Hora de início da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="12b2b-121">Start time of the time window</span></span>|
|<span data-ttu-id="12b2b-122">endTime</span><span class="sxs-lookup"><span data-stu-id="12b2b-122">endTime</span></span>|<span data-ttu-id="12b2b-123">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12b2b-123">TimeOfDay</span></span>|<span data-ttu-id="12b2b-124">Hora de término da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="12b2b-124">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="12b2b-125">Relações</span><span class="sxs-lookup"><span data-stu-id="12b2b-125">Relationships</span></span>
<span data-ttu-id="12b2b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12b2b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12b2b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12b2b-127">JSON Representation</span></span>
<span data-ttu-id="12b2b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12b2b-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



