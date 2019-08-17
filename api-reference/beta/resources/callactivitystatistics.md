---
title: tipo de recurso callActivityStatistics
description: Representa informações sobre as atividades de chamada para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 014cec3f8adab9f8d41b9f3062b38898b9956bb6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450705"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="a2378-103">tipo de recurso callActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="a2378-103">callActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2378-104">Representa dados sobre o tempo gasto pelo usuário em atividades de chamada no Microsoft Teams ou no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="a2378-104">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="a2378-105">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="a2378-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a2378-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2378-106">Properties</span></span>

| <span data-ttu-id="a2378-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2378-107">Property</span></span>     | <span data-ttu-id="a2378-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2378-108">Type</span></span>        | <span data-ttu-id="a2378-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2378-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2378-110">atividade</span><span class="sxs-lookup"><span data-stu-id="a2378-110">activity</span></span>|<span data-ttu-id="a2378-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="a2378-111">analyticsActivityType</span></span>| <span data-ttu-id="a2378-112">Atividade de chamada para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="a2378-112">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="a2378-113">duration</span><span class="sxs-lookup"><span data-stu-id="a2378-113">duration</span></span>|<span data-ttu-id="a2378-114">Duração</span><span class="sxs-lookup"><span data-stu-id="a2378-114">Duration</span></span>|<span data-ttu-id="a2378-115">Total de horas gasto em chamadas.</span><span class="sxs-lookup"><span data-stu-id="a2378-115">Total hours spent on calls.</span></span> <span data-ttu-id="a2378-116">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="a2378-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="a2378-117">endDate</span><span class="sxs-lookup"><span data-stu-id="a2378-117">endDate</span></span>|<span data-ttu-id="a2378-118">Data</span><span class="sxs-lookup"><span data-stu-id="a2378-118">Date</span></span>|<span data-ttu-id="a2378-119">Data de término da atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="a2378-119">Date when the call activity ended.</span></span> <span data-ttu-id="a2378-120">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="a2378-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="a2378-121">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a2378-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="a2378-122">id</span><span class="sxs-lookup"><span data-stu-id="a2378-122">id</span></span>|<span data-ttu-id="a2378-123">String</span><span class="sxs-lookup"><span data-stu-id="a2378-123">String</span></span>| <span data-ttu-id="a2378-124">Somente leitura ID para a atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="a2378-124">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="a2378-125">startDate</span><span class="sxs-lookup"><span data-stu-id="a2378-125">startDate</span></span>|<span data-ttu-id="a2378-126">Date</span><span class="sxs-lookup"><span data-stu-id="a2378-126">Date</span></span>|<span data-ttu-id="a2378-127">Data de início da atividade de chamada.</span><span class="sxs-lookup"><span data-stu-id="a2378-127">Date when the call activity started.</span></span> <span data-ttu-id="a2378-128">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="a2378-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="a2378-129">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a2378-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="a2378-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="a2378-130">timeZoneUsed</span></span>|<span data-ttu-id="a2378-131">String</span><span class="sxs-lookup"><span data-stu-id="a2378-131">String</span></span>|<span data-ttu-id="a2378-132">O fuso horário que o usuário define no calendário do Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="a2378-132">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="a2378-133">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="a2378-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="a2378-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="a2378-134">afterHours</span></span>|<span data-ttu-id="a2378-135">Duração</span><span class="sxs-lookup"><span data-stu-id="a2378-135">Duration</span></span>|<span data-ttu-id="a2378-136">Tempo gasto em chamadas fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2378-136">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="a2378-137">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="a2378-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2378-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a2378-138">Relationships</span></span>

<span data-ttu-id="a2378-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2378-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2378-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2378-140">JSON representation</span></span>

<span data-ttu-id="a2378-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2378-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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