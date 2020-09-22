---
title: tipo de recurso customUpdateTimeWindow
description: Janela de tempo de atualização personalizada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42f1be3ab2d3c345f7af5d91fd3bf1e6cc12865a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061977"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="ea511-103">tipo de recurso customUpdateTimeWindow</span><span class="sxs-lookup"><span data-stu-id="ea511-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="ea511-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea511-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea511-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea511-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea511-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea511-107">Janela de tempo de atualização personalizada</span><span class="sxs-lookup"><span data-stu-id="ea511-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="ea511-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea511-108">Properties</span></span>
|<span data-ttu-id="ea511-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea511-109">Property</span></span>|<span data-ttu-id="ea511-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea511-110">Type</span></span>|<span data-ttu-id="ea511-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea511-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea511-112">startDay</span><span class="sxs-lookup"><span data-stu-id="ea511-112">startDay</span></span>|[<span data-ttu-id="ea511-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="ea511-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="ea511-114">Dia inicial da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="ea511-114">Start day of the time window.</span></span> <span data-ttu-id="ea511-115">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="ea511-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ea511-116">endDay</span><span class="sxs-lookup"><span data-stu-id="ea511-116">endDay</span></span>|[<span data-ttu-id="ea511-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="ea511-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="ea511-118">Dia de término da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="ea511-118">End day of the time window.</span></span> <span data-ttu-id="ea511-119">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="ea511-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ea511-120">startTime</span><span class="sxs-lookup"><span data-stu-id="ea511-120">startTime</span></span>|<span data-ttu-id="ea511-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ea511-121">TimeOfDay</span></span>|<span data-ttu-id="ea511-122">Hora de início da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="ea511-122">Start time of the time window</span></span>|
|<span data-ttu-id="ea511-123">endTime</span><span class="sxs-lookup"><span data-stu-id="ea511-123">endTime</span></span>|<span data-ttu-id="ea511-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ea511-124">TimeOfDay</span></span>|<span data-ttu-id="ea511-125">Hora de término da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="ea511-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea511-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ea511-126">Relationships</span></span>
<span data-ttu-id="ea511-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea511-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea511-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea511-128">JSON Representation</span></span>
<span data-ttu-id="ea511-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea511-129">Here is a JSON representation of the resource.</span></span>
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






