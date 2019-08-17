---
title: tipo de recurso focusActivityStatistics
description: Representa informações sobre o trabalho de foco individual para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fc4431ac20c961569ce5cfaa607c2d2ab77240ee
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450692"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="21e3f-103">tipo de recurso focusActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="21e3f-103">focusActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21e3f-104">Representa dados sobre o tempo do usuário disponível para trabalho de foco.</span><span class="sxs-lookup"><span data-stu-id="21e3f-104">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="21e3f-105">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="21e3f-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21e3f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21e3f-106">Properties</span></span>

| <span data-ttu-id="21e3f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21e3f-107">Property</span></span>     | <span data-ttu-id="21e3f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="21e3f-108">Type</span></span>        | <span data-ttu-id="21e3f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e3f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21e3f-110">atividade</span><span class="sxs-lookup"><span data-stu-id="21e3f-110">activity</span></span>|<span data-ttu-id="21e3f-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="21e3f-111">analyticsActivityType</span></span>| <span data-ttu-id="21e3f-112">Atividade de foco para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="21e3f-112">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="21e3f-113">duration</span><span class="sxs-lookup"><span data-stu-id="21e3f-113">duration</span></span>|<span data-ttu-id="21e3f-114">Duração</span><span class="sxs-lookup"><span data-stu-id="21e3f-114">Duration</span></span>|<span data-ttu-id="21e3f-115">Soma total de horas de foco, que é igual a todos os blocos de tempo de pelo menos duas horas consecutivas, no calendário do Microsoft Outlook de um usuário sem uma reunião com outras pessoas dentro do horário de trabalho definido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21e3f-115">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="21e3f-116">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="21e3f-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="21e3f-117">endDate</span><span class="sxs-lookup"><span data-stu-id="21e3f-117">endDate</span></span>|<span data-ttu-id="21e3f-118">Data</span><span class="sxs-lookup"><span data-stu-id="21e3f-118">Date</span></span>|<span data-ttu-id="21e3f-119">Data de término da atividade de foco.</span><span class="sxs-lookup"><span data-stu-id="21e3f-119">Date when the focus activity ended.</span></span> <span data-ttu-id="21e3f-120">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="21e3f-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="21e3f-121">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="21e3f-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="21e3f-122">id</span><span class="sxs-lookup"><span data-stu-id="21e3f-122">id</span></span>|<span data-ttu-id="21e3f-123">String</span><span class="sxs-lookup"><span data-stu-id="21e3f-123">String</span></span>| <span data-ttu-id="21e3f-124">Somente leitura ID para a atividade Focus.</span><span class="sxs-lookup"><span data-stu-id="21e3f-124">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="21e3f-125">startDate</span><span class="sxs-lookup"><span data-stu-id="21e3f-125">startDate</span></span>|<span data-ttu-id="21e3f-126">Date</span><span class="sxs-lookup"><span data-stu-id="21e3f-126">Date</span></span>|<span data-ttu-id="21e3f-127">Data de início da atividade de foco.</span><span class="sxs-lookup"><span data-stu-id="21e3f-127">Date when the focus activity started.</span></span> <span data-ttu-id="21e3f-128">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="21e3f-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="21e3f-129">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="21e3f-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="21e3f-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="21e3f-130">timeZoneUsed</span></span>|<span data-ttu-id="21e3f-131">String</span><span class="sxs-lookup"><span data-stu-id="21e3f-131">String</span></span>|<span data-ttu-id="21e3f-132">O fuso horário que o usuário define no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="21e3f-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="21e3f-133">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="21e3f-133">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="21e3f-134">Relações</span><span class="sxs-lookup"><span data-stu-id="21e3f-134">Relationships</span></span>

<span data-ttu-id="21e3f-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21e3f-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21e3f-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21e3f-136">JSON representation</span></span>

<span data-ttu-id="21e3f-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21e3f-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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