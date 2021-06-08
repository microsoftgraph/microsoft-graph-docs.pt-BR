---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno para o tempo limite.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786065"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="59eb2-103">Tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="59eb2-103">timeOffRequest resource type</span></span>

<span data-ttu-id="59eb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59eb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59eb2-105">Representa um tipo de solicitação de turno para [fazer timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="59eb2-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="59eb2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="59eb2-106">Methods</span></span>

| <span data-ttu-id="59eb2-107">Método</span><span class="sxs-lookup"><span data-stu-id="59eb2-107">Method</span></span>       | <span data-ttu-id="59eb2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="59eb2-108">Return type</span></span> | <span data-ttu-id="59eb2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="59eb2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="59eb2-110">List</span><span class="sxs-lookup"><span data-stu-id="59eb2-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="59eb2-111">[Coleção timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="59eb2-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="59eb2-112">Obter a lista de **objetos timeOffRequest** nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="59eb2-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="59eb2-113">Get</span><span class="sxs-lookup"><span data-stu-id="59eb2-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="59eb2-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="59eb2-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="59eb2-115">Leia as propriedades e as relações de um **objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="59eb2-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="59eb2-116">Delete</span><span class="sxs-lookup"><span data-stu-id="59eb2-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="59eb2-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="59eb2-117">None</span></span> | <span data-ttu-id="59eb2-118">**Exclua um objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="59eb2-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="59eb2-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="59eb2-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="59eb2-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="59eb2-120">None</span></span>|<span data-ttu-id="59eb2-121">Aprovar uma solicitação de tempo de folga.</span><span class="sxs-lookup"><span data-stu-id="59eb2-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="59eb2-122">Declínio</span><span class="sxs-lookup"><span data-stu-id="59eb2-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="59eb2-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="59eb2-123">None</span></span>|<span data-ttu-id="59eb2-124">Recusar uma solicitação de tempo de folga.</span><span class="sxs-lookup"><span data-stu-id="59eb2-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="59eb2-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59eb2-125">Properties</span></span>

| <span data-ttu-id="59eb2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59eb2-126">Property</span></span>     | <span data-ttu-id="59eb2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="59eb2-127">Type</span></span>        | <span data-ttu-id="59eb2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="59eb2-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59eb2-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59eb2-129">endDateTime</span></span>|<span data-ttu-id="59eb2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59eb2-130">DateTimeOffset</span></span>|<span data-ttu-id="59eb2-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="59eb2-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="59eb2-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="59eb2-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="59eb2-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59eb2-133">startDateTime</span></span>|<span data-ttu-id="59eb2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59eb2-134">DateTimeOffset</span></span>|<span data-ttu-id="59eb2-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="59eb2-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="59eb2-136">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="59eb2-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="59eb2-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="59eb2-137">timeOffReasonId</span></span>|<span data-ttu-id="59eb2-138">String</span><span class="sxs-lookup"><span data-stu-id="59eb2-138">String</span></span>|<span data-ttu-id="59eb2-139">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="59eb2-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59eb2-140">Relações</span><span class="sxs-lookup"><span data-stu-id="59eb2-140">Relationships</span></span>

<span data-ttu-id="59eb2-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59eb2-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59eb2-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59eb2-142">JSON representation</span></span>

<span data-ttu-id="59eb2-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59eb2-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


