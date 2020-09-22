---
title: tipo de recurso emailActivityStatistics
description: Representa informações adicionais sobre atividades de email para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: af0fbc4247e7ffc9c8285409789d0437d8e09cb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055509"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="7f34f-103">tipo de recurso emailActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="7f34f-103">emailActivityStatistics resource type</span></span>

<span data-ttu-id="7f34f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f34f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f34f-105">Representa dados sobre o tempo gasto pelo usuário em atividades de email no Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f34f-105">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="7f34f-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="7f34f-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7f34f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f34f-107">Properties</span></span>

| <span data-ttu-id="7f34f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f34f-108">Property</span></span>     | <span data-ttu-id="7f34f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f34f-109">Type</span></span>        | <span data-ttu-id="7f34f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f34f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f34f-111">atividade</span><span class="sxs-lookup"><span data-stu-id="7f34f-111">activity</span></span>|<span data-ttu-id="7f34f-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="7f34f-112">analyticsActivityType</span></span>| <span data-ttu-id="7f34f-113">Atividade de email para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="7f34f-113">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="7f34f-114">duration</span><span class="sxs-lookup"><span data-stu-id="7f34f-114">duration</span></span>|<span data-ttu-id="7f34f-115">Duração</span><span class="sxs-lookup"><span data-stu-id="7f34f-115">Duration</span></span>|<span data-ttu-id="7f34f-116">Total de horas gasto nos emails.</span><span class="sxs-lookup"><span data-stu-id="7f34f-116">Total hours spent on emails.</span></span> <span data-ttu-id="7f34f-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="7f34f-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="7f34f-118">endDate</span><span class="sxs-lookup"><span data-stu-id="7f34f-118">endDate</span></span>|<span data-ttu-id="7f34f-119">Data</span><span class="sxs-lookup"><span data-stu-id="7f34f-119">Date</span></span>|<span data-ttu-id="7f34f-120">Data de término da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="7f34f-120">Date when the email activity ended.</span></span> <span data-ttu-id="7f34f-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="7f34f-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="7f34f-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7f34f-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="7f34f-123">id</span><span class="sxs-lookup"><span data-stu-id="7f34f-123">id</span></span>|<span data-ttu-id="7f34f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f34f-124">String</span></span>| <span data-ttu-id="7f34f-125">ID somente leitura da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="7f34f-125">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="7f34f-126">startDate</span><span class="sxs-lookup"><span data-stu-id="7f34f-126">startDate</span></span>|<span data-ttu-id="7f34f-127">Data</span><span class="sxs-lookup"><span data-stu-id="7f34f-127">Date</span></span>|<span data-ttu-id="7f34f-128">Data de início da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="7f34f-128">Date when the email activity started.</span></span> <span data-ttu-id="7f34f-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="7f34f-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="7f34f-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7f34f-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="7f34f-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="7f34f-131">timeZoneUsed</span></span>|<span data-ttu-id="7f34f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f34f-132">String</span></span>|<span data-ttu-id="7f34f-133">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="7f34f-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="7f34f-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="7f34f-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="7f34f-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="7f34f-135">afterHours</span></span>|<span data-ttu-id="7f34f-136">Duração</span><span class="sxs-lookup"><span data-stu-id="7f34f-136">Duration</span></span>|<span data-ttu-id="7f34f-137">Total de horas gasto no email fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7f34f-137">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="7f34f-138">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="7f34f-138">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="7f34f-139">readEmail</span><span class="sxs-lookup"><span data-stu-id="7f34f-139">readEmail</span></span>|<span data-ttu-id="7f34f-140">Duração</span><span class="sxs-lookup"><span data-stu-id="7f34f-140">Duration</span></span>|<span data-ttu-id="7f34f-141">Total de horas gasto na leitura de email.</span><span class="sxs-lookup"><span data-stu-id="7f34f-141">Total hours spent reading email.</span></span> <span data-ttu-id="7f34f-142">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="7f34f-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="7f34f-143">sentEmail</span><span class="sxs-lookup"><span data-stu-id="7f34f-143">sentEmail</span></span>|<span data-ttu-id="7f34f-144">Duração</span><span class="sxs-lookup"><span data-stu-id="7f34f-144">Duration</span></span>|<span data-ttu-id="7f34f-145">Total de horas gasto na gravação e envio de email.</span><span class="sxs-lookup"><span data-stu-id="7f34f-145">Total hours spent writing and sending email.</span></span> <span data-ttu-id="7f34f-146">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="7f34f-146">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f34f-147">Relações</span><span class="sxs-lookup"><span data-stu-id="7f34f-147">Relationships</span></span>

<span data-ttu-id="7f34f-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f34f-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f34f-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f34f-149">JSON representation</span></span>

<span data-ttu-id="7f34f-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f34f-150">The following is a JSON representation of the resource.</span></span>

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

