---
title: tipo de recurso chatActivityStatistics
description: Representa informações sobre atividades de chat para usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a380ef18435ca971da4f3163fc1268ec7f28e565
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064343"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="e5e83-103">tipo de recurso chatActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="e5e83-103">chatActivityStatistics resource type</span></span>

<span data-ttu-id="e5e83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5e83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5e83-105">Representa dados sobre o tempo gasto pelo usuário em atividades de chat no Microsoft Teams ou no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="e5e83-105">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="e5e83-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="e5e83-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e5e83-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5e83-107">Properties</span></span>

| <span data-ttu-id="e5e83-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5e83-108">Property</span></span>     | <span data-ttu-id="e5e83-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5e83-109">Type</span></span>        | <span data-ttu-id="e5e83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5e83-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5e83-111">atividade</span><span class="sxs-lookup"><span data-stu-id="e5e83-111">activity</span></span>|<span data-ttu-id="e5e83-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="e5e83-112">analyticsActivityType</span></span>| <span data-ttu-id="e5e83-113">Atividade de chat para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="e5e83-113">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="e5e83-114">duration</span><span class="sxs-lookup"><span data-stu-id="e5e83-114">duration</span></span>|<span data-ttu-id="e5e83-115">Duração</span><span class="sxs-lookup"><span data-stu-id="e5e83-115">Duration</span></span>|<span data-ttu-id="e5e83-116">Total de horas gasto em chats.</span><span class="sxs-lookup"><span data-stu-id="e5e83-116">Total hours spent on chats.</span></span> <span data-ttu-id="e5e83-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="e5e83-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="e5e83-118">endDate</span><span class="sxs-lookup"><span data-stu-id="e5e83-118">endDate</span></span>|<span data-ttu-id="e5e83-119">Data</span><span class="sxs-lookup"><span data-stu-id="e5e83-119">Date</span></span>|<span data-ttu-id="e5e83-120">Data de término da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="e5e83-120">Date when the chat activity ended.</span></span> <span data-ttu-id="e5e83-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="e5e83-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e5e83-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e5e83-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e5e83-123">id</span><span class="sxs-lookup"><span data-stu-id="e5e83-123">id</span></span>|<span data-ttu-id="e5e83-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5e83-124">String</span></span>| <span data-ttu-id="e5e83-125">ID somente leitura da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="e5e83-125">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="e5e83-126">startDate</span><span class="sxs-lookup"><span data-stu-id="e5e83-126">startDate</span></span>|<span data-ttu-id="e5e83-127">Data</span><span class="sxs-lookup"><span data-stu-id="e5e83-127">Date</span></span>|<span data-ttu-id="e5e83-128">Data de início da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="e5e83-128">Date when the chat activity started.</span></span> <span data-ttu-id="e5e83-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="e5e83-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e5e83-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e5e83-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e5e83-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="e5e83-131">timeZoneUsed</span></span>|<span data-ttu-id="e5e83-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5e83-132">String</span></span>|<span data-ttu-id="e5e83-133">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="e5e83-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="e5e83-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="e5e83-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="e5e83-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="e5e83-135">afterHours</span></span>|<span data-ttu-id="e5e83-136">Duração</span><span class="sxs-lookup"><span data-stu-id="e5e83-136">Duration</span></span>|<span data-ttu-id="e5e83-137">Tempo gasto em chats fora do horário de trabalho, que se baseia na configuração de calendário do Microsoft Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e5e83-137">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="e5e83-138">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="e5e83-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e5e83-139">Relações</span><span class="sxs-lookup"><span data-stu-id="e5e83-139">Relationships</span></span>

<span data-ttu-id="e5e83-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5e83-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5e83-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5e83-141">JSON representation</span></span>

<span data-ttu-id="e5e83-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5e83-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatActivityStatistics"
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
  "description": "chatActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



