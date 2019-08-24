---
title: tipo de recurso emailActivityStatistics
description: Representa informações adicionais sobre atividades de email para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: d4f9cd2e8608a29a34ccd0c8bdf54fafa77fee33
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622611"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="f1d37-103">tipo de recurso emailActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="f1d37-103">emailActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d37-104">Representa dados sobre o tempo gasto pelo usuário em atividades de email no Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="f1d37-104">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="f1d37-105">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="f1d37-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f1d37-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1d37-106">Properties</span></span>

| <span data-ttu-id="f1d37-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1d37-107">Property</span></span>     | <span data-ttu-id="f1d37-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1d37-108">Type</span></span>        | <span data-ttu-id="f1d37-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1d37-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1d37-110">atividade</span><span class="sxs-lookup"><span data-stu-id="f1d37-110">activity</span></span>|<span data-ttu-id="f1d37-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="f1d37-111">analyticsActivityType</span></span>| <span data-ttu-id="f1d37-112">Atividade de email para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f1d37-112">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="f1d37-113">duration</span><span class="sxs-lookup"><span data-stu-id="f1d37-113">duration</span></span>|<span data-ttu-id="f1d37-114">Duração</span><span class="sxs-lookup"><span data-stu-id="f1d37-114">Duration</span></span>|<span data-ttu-id="f1d37-115">Total de horas gasto nos emails.</span><span class="sxs-lookup"><span data-stu-id="f1d37-115">Total hours spent on emails.</span></span> <span data-ttu-id="f1d37-116">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="f1d37-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="f1d37-117">endDate</span><span class="sxs-lookup"><span data-stu-id="f1d37-117">endDate</span></span>|<span data-ttu-id="f1d37-118">Data</span><span class="sxs-lookup"><span data-stu-id="f1d37-118">Date</span></span>|<span data-ttu-id="f1d37-119">Data de término da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="f1d37-119">Date when the email activity ended.</span></span> <span data-ttu-id="f1d37-120">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="f1d37-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f1d37-121">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f1d37-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f1d37-122">id</span><span class="sxs-lookup"><span data-stu-id="f1d37-122">id</span></span>|<span data-ttu-id="f1d37-123">String</span><span class="sxs-lookup"><span data-stu-id="f1d37-123">String</span></span>| <span data-ttu-id="f1d37-124">ID somente leitura da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="f1d37-124">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="f1d37-125">startDate</span><span class="sxs-lookup"><span data-stu-id="f1d37-125">startDate</span></span>|<span data-ttu-id="f1d37-126">Date</span><span class="sxs-lookup"><span data-stu-id="f1d37-126">Date</span></span>|<span data-ttu-id="f1d37-127">Data de início da atividade de email.</span><span class="sxs-lookup"><span data-stu-id="f1d37-127">Date when the email activity started.</span></span> <span data-ttu-id="f1d37-128">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="f1d37-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="f1d37-129">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f1d37-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="f1d37-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="f1d37-130">timeZoneUsed</span></span>|<span data-ttu-id="f1d37-131">String</span><span class="sxs-lookup"><span data-stu-id="f1d37-131">String</span></span>|<span data-ttu-id="f1d37-132">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="f1d37-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="f1d37-133">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="f1d37-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="f1d37-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="f1d37-134">afterHours</span></span>|<span data-ttu-id="f1d37-135">Duração</span><span class="sxs-lookup"><span data-stu-id="f1d37-135">Duration</span></span>|<span data-ttu-id="f1d37-136">Total de horas gasto no email fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f1d37-136">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="f1d37-137">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="f1d37-137">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="f1d37-138">readEmail</span><span class="sxs-lookup"><span data-stu-id="f1d37-138">readEmail</span></span>|<span data-ttu-id="f1d37-139">Duração</span><span class="sxs-lookup"><span data-stu-id="f1d37-139">Duration</span></span>|<span data-ttu-id="f1d37-140">Total de horas gasto na leitura de email.</span><span class="sxs-lookup"><span data-stu-id="f1d37-140">Total hours spent reading email.</span></span> <span data-ttu-id="f1d37-141">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="f1d37-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="f1d37-142">sentEmail</span><span class="sxs-lookup"><span data-stu-id="f1d37-142">sentEmail</span></span>|<span data-ttu-id="f1d37-143">Duração</span><span class="sxs-lookup"><span data-stu-id="f1d37-143">Duration</span></span>|<span data-ttu-id="f1d37-144">Total de horas gasto na gravação e envio de email.</span><span class="sxs-lookup"><span data-stu-id="f1d37-144">Total hours spent writing and sending email.</span></span> <span data-ttu-id="f1d37-145">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="f1d37-145">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1d37-146">Relações</span><span class="sxs-lookup"><span data-stu-id="f1d37-146">Relationships</span></span>

<span data-ttu-id="f1d37-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1d37-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1d37-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1d37-148">JSON representation</span></span>

<span data-ttu-id="f1d37-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1d37-149">The following is a JSON representation of the resource.</span></span>

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