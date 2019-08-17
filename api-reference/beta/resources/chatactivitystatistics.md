---
title: tipo de recurso chatActivityStatistics
description: Representa informações sobre atividades de chat para usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 53822af8af2426cb8100cbf8a9cb417757d72e14
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450697"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="08d8d-103">tipo de recurso chatActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="08d8d-103">chatActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08d8d-104">Representa dados sobre o tempo gasto pelo usuário em atividades de chat no Microsoft Teams ou no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="08d8d-104">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="08d8d-105">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="08d8d-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="08d8d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08d8d-106">Properties</span></span>

| <span data-ttu-id="08d8d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08d8d-107">Property</span></span>     | <span data-ttu-id="08d8d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="08d8d-108">Type</span></span>        | <span data-ttu-id="08d8d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d8d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08d8d-110">atividade</span><span class="sxs-lookup"><span data-stu-id="08d8d-110">activity</span></span>|<span data-ttu-id="08d8d-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="08d8d-111">analyticsActivityType</span></span>| <span data-ttu-id="08d8d-112">Atividade de chat para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="08d8d-112">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="08d8d-113">duration</span><span class="sxs-lookup"><span data-stu-id="08d8d-113">duration</span></span>|<span data-ttu-id="08d8d-114">Duração</span><span class="sxs-lookup"><span data-stu-id="08d8d-114">Duration</span></span>|<span data-ttu-id="08d8d-115">Total de horas gasto em chats.</span><span class="sxs-lookup"><span data-stu-id="08d8d-115">Total hours spent on chats.</span></span> <span data-ttu-id="08d8d-116">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="08d8d-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="08d8d-117">endDate</span><span class="sxs-lookup"><span data-stu-id="08d8d-117">endDate</span></span>|<span data-ttu-id="08d8d-118">Data</span><span class="sxs-lookup"><span data-stu-id="08d8d-118">Date</span></span>|<span data-ttu-id="08d8d-119">Data de término da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="08d8d-119">Date when the chat activity ended.</span></span> <span data-ttu-id="08d8d-120">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="08d8d-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="08d8d-121">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="08d8d-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="08d8d-122">id</span><span class="sxs-lookup"><span data-stu-id="08d8d-122">id</span></span>|<span data-ttu-id="08d8d-123">String</span><span class="sxs-lookup"><span data-stu-id="08d8d-123">String</span></span>| <span data-ttu-id="08d8d-124">ID somente leitura da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="08d8d-124">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="08d8d-125">startDate</span><span class="sxs-lookup"><span data-stu-id="08d8d-125">startDate</span></span>|<span data-ttu-id="08d8d-126">Date</span><span class="sxs-lookup"><span data-stu-id="08d8d-126">Date</span></span>|<span data-ttu-id="08d8d-127">Data de início da atividade de chat.</span><span class="sxs-lookup"><span data-stu-id="08d8d-127">Date when the chat activity started.</span></span> <span data-ttu-id="08d8d-128">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="08d8d-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="08d8d-129">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="08d8d-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="08d8d-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="08d8d-130">timeZoneUsed</span></span>|<span data-ttu-id="08d8d-131">String</span><span class="sxs-lookup"><span data-stu-id="08d8d-131">String</span></span>|<span data-ttu-id="08d8d-132">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="08d8d-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="08d8d-133">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="08d8d-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="08d8d-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="08d8d-134">afterHours</span></span>|<span data-ttu-id="08d8d-135">Duração</span><span class="sxs-lookup"><span data-stu-id="08d8d-135">Duration</span></span>|<span data-ttu-id="08d8d-136">Tempo gasto em chats fora do horário de trabalho, que se baseia na configuração de calendário do Microsoft Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="08d8d-136">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="08d8d-137">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="08d8d-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="08d8d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="08d8d-138">Relationships</span></span>

<span data-ttu-id="08d8d-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08d8d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08d8d-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08d8d-140">JSON representation</span></span>

<span data-ttu-id="08d8d-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08d8d-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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

