---
title: tipo de recurso callActivityStatistics
description: Representa informações sobre as atividades de chamada para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8d7eb23fc0ed148b38f3cb7adb29d8af49fa7400
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071512"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="8d019-103">tipo de recurso callActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="8d019-103">callActivityStatistics resource type</span></span>

<span data-ttu-id="8d019-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d019-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d019-105">Representa dados sobre o tempo gasto pelo usuário em atividades de chamada no Microsoft Teams ou no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="8d019-105">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="8d019-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="8d019-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d019-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d019-107">Properties</span></span>

| <span data-ttu-id="8d019-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d019-108">Property</span></span>     | <span data-ttu-id="8d019-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d019-109">Type</span></span>        | <span data-ttu-id="8d019-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d019-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d019-111">atividade</span><span class="sxs-lookup"><span data-stu-id="8d019-111">activity</span></span>|<span data-ttu-id="8d019-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="8d019-112">analyticsActivityType</span></span>| <span data-ttu-id="8d019-113">Atividade de chamada para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8d019-113">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="8d019-114">duration</span><span class="sxs-lookup"><span data-stu-id="8d019-114">duration</span></span>|<span data-ttu-id="8d019-115">Duração</span><span class="sxs-lookup"><span data-stu-id="8d019-115">Duration</span></span>|<span data-ttu-id="8d019-116">Total de horas gasto em chamadas.</span><span class="sxs-lookup"><span data-stu-id="8d019-116">Total hours spent on calls.</span></span> <span data-ttu-id="8d019-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="8d019-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="8d019-118">endDate</span><span class="sxs-lookup"><span data-stu-id="8d019-118">endDate</span></span>|<span data-ttu-id="8d019-119">Data</span><span class="sxs-lookup"><span data-stu-id="8d019-119">Date</span></span>|<span data-ttu-id="8d019-120">Data de término da atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="8d019-120">Date when the call activity ended.</span></span> <span data-ttu-id="8d019-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="8d019-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="8d019-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="8d019-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="8d019-123">id</span><span class="sxs-lookup"><span data-stu-id="8d019-123">id</span></span>|<span data-ttu-id="8d019-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d019-124">String</span></span>| <span data-ttu-id="8d019-125">Somente leitura ID para a atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="8d019-125">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="8d019-126">startDate</span><span class="sxs-lookup"><span data-stu-id="8d019-126">startDate</span></span>|<span data-ttu-id="8d019-127">Data</span><span class="sxs-lookup"><span data-stu-id="8d019-127">Date</span></span>|<span data-ttu-id="8d019-128">Data de início da atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="8d019-128">Date when the call activity started.</span></span> <span data-ttu-id="8d019-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="8d019-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="8d019-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="8d019-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="8d019-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="8d019-131">timeZoneUsed</span></span>|<span data-ttu-id="8d019-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d019-132">String</span></span>|<span data-ttu-id="8d019-133">O fuso horário que o usuário define no calendário do Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="8d019-133">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="8d019-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="8d019-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="8d019-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="8d019-135">afterHours</span></span>|<span data-ttu-id="8d019-136">Duração</span><span class="sxs-lookup"><span data-stu-id="8d019-136">Duration</span></span>|<span data-ttu-id="8d019-137">Tempo gasto em chamadas fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8d019-137">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="8d019-138">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="8d019-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d019-139">Relações</span><span class="sxs-lookup"><span data-stu-id="8d019-139">Relationships</span></span>

<span data-ttu-id="8d019-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d019-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d019-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d019-141">JSON representation</span></span>

<span data-ttu-id="8d019-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d019-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

