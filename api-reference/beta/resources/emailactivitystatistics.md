---
title: tipo de recurso emailActivityStatistics
description: Representa informações adicionais sobre atividades de email para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f2bd2d84d6f7dbc18fc5e37079eebc4289dd2ee2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499593"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="2ef2a-103">tipo de recurso emailActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="2ef2a-103">emailActivityStatistics resource type</span></span>

<span data-ttu-id="2ef2a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef2a-105">Representa dados sobre o tempo gasto pelo usuário em atividades de email no Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-105">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="2ef2a-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="2ef2a-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2ef2a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ef2a-107">Properties</span></span>

| <span data-ttu-id="2ef2a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef2a-108">Property</span></span>     | <span data-ttu-id="2ef2a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef2a-109">Type</span></span>        | <span data-ttu-id="2ef2a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef2a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ef2a-111">atividade</span><span class="sxs-lookup"><span data-stu-id="2ef2a-111">activity</span></span>|<span data-ttu-id="2ef2a-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="2ef2a-112">analyticsActivityType</span></span>| <span data-ttu-id="2ef2a-113">Atividade de email para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-113">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="2ef2a-114">duration</span><span class="sxs-lookup"><span data-stu-id="2ef2a-114">duration</span></span>|<span data-ttu-id="2ef2a-115">Duração</span><span class="sxs-lookup"><span data-stu-id="2ef2a-115">Duration</span></span>|<span data-ttu-id="2ef2a-116">Total de horas gasto nos emails.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-116">Total hours spent on emails.</span></span> <span data-ttu-id="2ef2a-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="2ef2a-118">endDate</span><span class="sxs-lookup"><span data-stu-id="2ef2a-118">endDate</span></span>|<span data-ttu-id="2ef2a-119">Data</span><span class="sxs-lookup"><span data-stu-id="2ef2a-119">Date</span></span>|<span data-ttu-id="2ef2a-120">Data de término da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-120">Date when the email activity ended.</span></span> <span data-ttu-id="2ef2a-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="2ef2a-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="2ef2a-123">id</span><span class="sxs-lookup"><span data-stu-id="2ef2a-123">id</span></span>|<span data-ttu-id="2ef2a-124">String</span><span class="sxs-lookup"><span data-stu-id="2ef2a-124">String</span></span>| <span data-ttu-id="2ef2a-125">ID somente leitura da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-125">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="2ef2a-126">startDate</span><span class="sxs-lookup"><span data-stu-id="2ef2a-126">startDate</span></span>|<span data-ttu-id="2ef2a-127">Date</span><span class="sxs-lookup"><span data-stu-id="2ef2a-127">Date</span></span>|<span data-ttu-id="2ef2a-128">Data de início da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-128">Date when the email activity started.</span></span> <span data-ttu-id="2ef2a-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="2ef2a-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="2ef2a-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="2ef2a-131">timeZoneUsed</span></span>|<span data-ttu-id="2ef2a-132">String</span><span class="sxs-lookup"><span data-stu-id="2ef2a-132">String</span></span>|<span data-ttu-id="2ef2a-133">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="2ef2a-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="2ef2a-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="2ef2a-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="2ef2a-135">afterHours</span></span>|<span data-ttu-id="2ef2a-136">Duração</span><span class="sxs-lookup"><span data-stu-id="2ef2a-136">Duration</span></span>|<span data-ttu-id="2ef2a-137">Total de horas gasto no email fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-137">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="2ef2a-138">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-138">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="2ef2a-139">readEmail</span><span class="sxs-lookup"><span data-stu-id="2ef2a-139">readEmail</span></span>|<span data-ttu-id="2ef2a-140">Duração</span><span class="sxs-lookup"><span data-stu-id="2ef2a-140">Duration</span></span>|<span data-ttu-id="2ef2a-141">Total de horas gasto na leitura de email.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-141">Total hours spent reading email.</span></span> <span data-ttu-id="2ef2a-142">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="2ef2a-143">sentEmail</span><span class="sxs-lookup"><span data-stu-id="2ef2a-143">sentEmail</span></span>|<span data-ttu-id="2ef2a-144">Duração</span><span class="sxs-lookup"><span data-stu-id="2ef2a-144">Duration</span></span>|<span data-ttu-id="2ef2a-145">Total de horas gasto na gravação e envio de email.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-145">Total hours spent writing and sending email.</span></span> <span data-ttu-id="2ef2a-146">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-146">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ef2a-147">Relações</span><span class="sxs-lookup"><span data-stu-id="2ef2a-147">Relationships</span></span>

<span data-ttu-id="2ef2a-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ef2a-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ef2a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ef2a-149">JSON representation</span></span>

<span data-ttu-id="2ef2a-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ef2a-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->