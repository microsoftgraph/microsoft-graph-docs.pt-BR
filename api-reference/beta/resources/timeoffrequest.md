---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno para o tempo limite.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 42ad70594dfc5f5c0491b88c95d88e19e226ec1c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720176"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="f2621-103">Tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="f2621-103">timeOffRequest resource type</span></span>

<span data-ttu-id="f2621-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2621-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2621-105">Representa um tipo de solicitação de turno para [o tempo limite](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="f2621-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f2621-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2621-106">Methods</span></span>

| <span data-ttu-id="f2621-107">Método</span><span class="sxs-lookup"><span data-stu-id="f2621-107">Method</span></span>       | <span data-ttu-id="f2621-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2621-108">Return Type</span></span> | <span data-ttu-id="f2621-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2621-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f2621-110">List</span><span class="sxs-lookup"><span data-stu-id="f2621-110">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="f2621-111">[Coleção timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f2621-111">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="f2621-112">Obter a lista de **objetos timeOffRequest** nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="f2621-112">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="f2621-113">Get</span><span class="sxs-lookup"><span data-stu-id="f2621-113">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="f2621-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="f2621-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="f2621-115">Leia as propriedades e as relações de um **objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="f2621-115">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="f2621-116">Delete</span><span class="sxs-lookup"><span data-stu-id="f2621-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="f2621-117">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="f2621-117">None</span></span> | <span data-ttu-id="f2621-118">**Exclua um objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="f2621-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="f2621-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="f2621-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="f2621-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="f2621-120">None</span></span>|<span data-ttu-id="f2621-121">Aprovar uma solicitação de tempo de folga.</span><span class="sxs-lookup"><span data-stu-id="f2621-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="f2621-122">Declínio</span><span class="sxs-lookup"><span data-stu-id="f2621-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="f2621-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="f2621-123">None</span></span>|<span data-ttu-id="f2621-124">Recusar uma solicitação de tempo de folga.</span><span class="sxs-lookup"><span data-stu-id="f2621-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2621-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2621-125">Properties</span></span>

| <span data-ttu-id="f2621-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2621-126">Property</span></span>     | <span data-ttu-id="f2621-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2621-127">Type</span></span>        | <span data-ttu-id="f2621-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2621-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2621-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f2621-129">endDateTime</span></span>|<span data-ttu-id="f2621-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2621-130">DateTimeOffset</span></span>|<span data-ttu-id="f2621-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f2621-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2621-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f2621-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f2621-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f2621-133">startDateTime</span></span>|<span data-ttu-id="f2621-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2621-134">DateTimeOffset</span></span>|<span data-ttu-id="f2621-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f2621-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2621-136">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f2621-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f2621-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="f2621-137">timeOffReasonId</span></span>|<span data-ttu-id="f2621-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2621-138">String</span></span>|<span data-ttu-id="f2621-139">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="f2621-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2621-140">Relações</span><span class="sxs-lookup"><span data-stu-id="f2621-140">Relationships</span></span>

<span data-ttu-id="f2621-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2621-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2621-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2621-142">JSON representation</span></span>

<span data-ttu-id="f2621-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2621-143">The following is a JSON representation of the resource.</span></span>

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


