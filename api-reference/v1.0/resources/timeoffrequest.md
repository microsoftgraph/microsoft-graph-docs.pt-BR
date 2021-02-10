---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno a ser timeOff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e234873110f50ed66decaa04b5462a9ff6fcf9a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154198"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="9c8a2-103">Tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="9c8a2-103">timeOffRequest resource type</span></span>

<span data-ttu-id="9c8a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c8a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c8a2-105">Representa um tipo de solicitação de turno para [tomar timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="9c8a2-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9c8a2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c8a2-106">Methods</span></span>

| <span data-ttu-id="9c8a2-107">Método</span><span class="sxs-lookup"><span data-stu-id="9c8a2-107">Method</span></span>       | <span data-ttu-id="9c8a2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c8a2-108">Return Type</span></span> | <span data-ttu-id="9c8a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c8a2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9c8a2-110">Get</span><span class="sxs-lookup"><span data-stu-id="9c8a2-110">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="9c8a2-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="9c8a2-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="9c8a2-112">Leia as propriedades e os relacionamentos de um **objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="9c8a2-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="9c8a2-113">Lista</span><span class="sxs-lookup"><span data-stu-id="9c8a2-113">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="9c8a2-114">[Coleção timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9c8a2-114">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="9c8a2-115">Obter a lista de **objetos timeOffRequest** nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="9c8a2-115">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="9c8a2-116">Delete</span><span class="sxs-lookup"><span data-stu-id="9c8a2-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="9c8a2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c8a2-117">None</span></span> | <span data-ttu-id="9c8a2-118">**Exclua um objeto timeOffRequest.**</span><span class="sxs-lookup"><span data-stu-id="9c8a2-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="9c8a2-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="9c8a2-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="9c8a2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c8a2-120">None</span></span>|<span data-ttu-id="9c8a2-121">Aprovar uma solicitação de folga.</span><span class="sxs-lookup"><span data-stu-id="9c8a2-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="9c8a2-122">Recusar</span><span class="sxs-lookup"><span data-stu-id="9c8a2-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="9c8a2-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c8a2-123">None</span></span>|<span data-ttu-id="9c8a2-124">Recusar uma solicitação de folga.</span><span class="sxs-lookup"><span data-stu-id="9c8a2-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c8a2-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c8a2-125">Properties</span></span>

| <span data-ttu-id="9c8a2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c8a2-126">Property</span></span>     | <span data-ttu-id="9c8a2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c8a2-127">Type</span></span>        | <span data-ttu-id="9c8a2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c8a2-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c8a2-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9c8a2-129">endDateTime</span></span>|<span data-ttu-id="9c8a2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c8a2-130">DateTimeOffset</span></span>|<span data-ttu-id="9c8a2-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9c8a2-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c8a2-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9c8a2-133">startDateTime</span></span>|<span data-ttu-id="9c8a2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c8a2-134">DateTimeOffset</span></span>|<span data-ttu-id="9c8a2-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9c8a2-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c8a2-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="9c8a2-137">timeOffReasonId</span></span>|<span data-ttu-id="9c8a2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c8a2-138">String</span></span>|<span data-ttu-id="9c8a2-139">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="9c8a2-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c8a2-140">Relações</span><span class="sxs-lookup"><span data-stu-id="9c8a2-140">Relationships</span></span>

<span data-ttu-id="9c8a2-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c8a2-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c8a2-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c8a2-142">JSON representation</span></span>

<span data-ttu-id="9c8a2-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c8a2-143">The following is a JSON representation of the resource.</span></span>

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

