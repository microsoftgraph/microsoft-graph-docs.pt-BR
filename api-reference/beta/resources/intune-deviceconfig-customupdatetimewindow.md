---
title: tipo de recurso customUpdateTimeWindow
description: Janela de tempo de atualização personalizada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7392ba0eeb3af516682ff63f9f65fce94d08f0e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729788"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="acec5-103">tipo de recurso customUpdateTimeWindow</span><span class="sxs-lookup"><span data-stu-id="acec5-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="acec5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acec5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acec5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="acec5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acec5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acec5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acec5-107">Janela de tempo de atualização personalizada</span><span class="sxs-lookup"><span data-stu-id="acec5-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="acec5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acec5-108">Properties</span></span>
|<span data-ttu-id="acec5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acec5-109">Property</span></span>|<span data-ttu-id="acec5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="acec5-110">Type</span></span>|<span data-ttu-id="acec5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="acec5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acec5-112">startDay</span><span class="sxs-lookup"><span data-stu-id="acec5-112">startDay</span></span>|[<span data-ttu-id="acec5-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="acec5-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="acec5-114">Dia inicial da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="acec5-114">Start day of the time window.</span></span> <span data-ttu-id="acec5-115">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="acec5-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="acec5-116">endDay</span><span class="sxs-lookup"><span data-stu-id="acec5-116">endDay</span></span>|[<span data-ttu-id="acec5-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="acec5-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="acec5-118">Dia de término da janela de tempo.</span><span class="sxs-lookup"><span data-stu-id="acec5-118">End day of the time window.</span></span> <span data-ttu-id="acec5-119">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="acec5-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="acec5-120">startTime</span><span class="sxs-lookup"><span data-stu-id="acec5-120">startTime</span></span>|<span data-ttu-id="acec5-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="acec5-121">TimeOfDay</span></span>|<span data-ttu-id="acec5-122">Hora de início da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="acec5-122">Start time of the time window</span></span>|
|<span data-ttu-id="acec5-123">endTime</span><span class="sxs-lookup"><span data-stu-id="acec5-123">endTime</span></span>|<span data-ttu-id="acec5-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="acec5-124">TimeOfDay</span></span>|<span data-ttu-id="acec5-125">Hora de término da janela de tempo</span><span class="sxs-lookup"><span data-stu-id="acec5-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="acec5-126">Relações</span><span class="sxs-lookup"><span data-stu-id="acec5-126">Relationships</span></span>
<span data-ttu-id="acec5-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acec5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acec5-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acec5-128">JSON Representation</span></span>
<span data-ttu-id="acec5-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acec5-129">Here is a JSON representation of the resource.</span></span>
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





