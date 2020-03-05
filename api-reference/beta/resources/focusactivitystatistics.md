---
title: tipo de recurso focusActivityStatistics
description: Representa informações sobre o trabalho de foco individual para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1c92225c0a95f49bd95b8c81abac70a0600f7cea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497990"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="61261-103">tipo de recurso focusActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="61261-103">focusActivityStatistics resource type</span></span>

<span data-ttu-id="61261-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61261-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61261-105">Representa dados sobre o tempo do usuário disponível para trabalho de foco.</span><span class="sxs-lookup"><span data-stu-id="61261-105">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="61261-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="61261-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="61261-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61261-107">Properties</span></span>

| <span data-ttu-id="61261-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61261-108">Property</span></span>     | <span data-ttu-id="61261-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="61261-109">Type</span></span>        | <span data-ttu-id="61261-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61261-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61261-111">atividade</span><span class="sxs-lookup"><span data-stu-id="61261-111">activity</span></span>|<span data-ttu-id="61261-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="61261-112">analyticsActivityType</span></span>| <span data-ttu-id="61261-113">Atividade de foco para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="61261-113">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="61261-114">duration</span><span class="sxs-lookup"><span data-stu-id="61261-114">duration</span></span>|<span data-ttu-id="61261-115">Duração</span><span class="sxs-lookup"><span data-stu-id="61261-115">Duration</span></span>|<span data-ttu-id="61261-116">Soma total de horas de foco, que é igual a todos os blocos de tempo de pelo menos duas horas consecutivas, no calendário do Microsoft Outlook de um usuário sem uma reunião com outras pessoas dentro do horário de trabalho definido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="61261-116">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="61261-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="61261-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="61261-118">endDate</span><span class="sxs-lookup"><span data-stu-id="61261-118">endDate</span></span>|<span data-ttu-id="61261-119">Data</span><span class="sxs-lookup"><span data-stu-id="61261-119">Date</span></span>|<span data-ttu-id="61261-120">Data de término da atividade de foco.</span><span class="sxs-lookup"><span data-stu-id="61261-120">Date when the focus activity ended.</span></span> <span data-ttu-id="61261-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="61261-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="61261-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="61261-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="61261-123">id</span><span class="sxs-lookup"><span data-stu-id="61261-123">id</span></span>|<span data-ttu-id="61261-124">String</span><span class="sxs-lookup"><span data-stu-id="61261-124">String</span></span>| <span data-ttu-id="61261-125">Somente leitura ID para a atividade Focus.</span><span class="sxs-lookup"><span data-stu-id="61261-125">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="61261-126">startDate</span><span class="sxs-lookup"><span data-stu-id="61261-126">startDate</span></span>|<span data-ttu-id="61261-127">Date</span><span class="sxs-lookup"><span data-stu-id="61261-127">Date</span></span>|<span data-ttu-id="61261-128">Data de início da atividade de foco.</span><span class="sxs-lookup"><span data-stu-id="61261-128">Date when the focus activity started.</span></span> <span data-ttu-id="61261-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="61261-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="61261-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="61261-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="61261-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="61261-131">timeZoneUsed</span></span>|<span data-ttu-id="61261-132">String</span><span class="sxs-lookup"><span data-stu-id="61261-132">String</span></span>|<span data-ttu-id="61261-133">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="61261-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="61261-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="61261-134">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="61261-135">Relações</span><span class="sxs-lookup"><span data-stu-id="61261-135">Relationships</span></span>

<span data-ttu-id="61261-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61261-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61261-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61261-137">JSON representation</span></span>

<span data-ttu-id="61261-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61261-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->