---
title: tipo de recurso segment
description: O tipo de segmento
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb95c665ed3967aeb9b18fcefd262ad52490306
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720225"
---
# <a name="segment-resource-type"></a><span data-ttu-id="188d3-103">tipo de recurso segment</span><span class="sxs-lookup"><span data-stu-id="188d3-103">segment resource type</span></span>

<span data-ttu-id="188d3-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="188d3-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="188d3-105">Representa uma parte de uma comunicação User-User ou uma User-Meeting no caso de uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="188d3-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="188d3-106">Uma chamada VOIP típica terá um segmento por sessão.</span><span class="sxs-lookup"><span data-stu-id="188d3-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="188d3-107">Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão devido à comunicação de servidor para servidor adicional necessária para conectar a chamada.</span><span class="sxs-lookup"><span data-stu-id="188d3-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="188d3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="188d3-108">Methods</span></span>

<span data-ttu-id="188d3-109">Não existem métodos para acessar diretamente segmentos.</span><span class="sxs-lookup"><span data-stu-id="188d3-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="188d3-110">Use a api [Get callRecord](../api/callrecords-callrecord-get.md) com ou a api de sessão list com para obter os `$expand=sessions($expand=segments)` [](../api/callrecords-session-list.md) `$expand=segments` segmentos de um [callRecord](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="188d3-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="188d3-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="188d3-111">Properties</span></span>

| <span data-ttu-id="188d3-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="188d3-112">Property</span></span>     | <span data-ttu-id="188d3-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="188d3-113">Type</span></span>        | <span data-ttu-id="188d3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="188d3-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="188d3-115">id</span><span class="sxs-lookup"><span data-stu-id="188d3-115">id</span></span>|<span data-ttu-id="188d3-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="188d3-116">String</span></span>|<span data-ttu-id="188d3-117">Identificador exclusivo do segmento.</span><span class="sxs-lookup"><span data-stu-id="188d3-117">Unique identifier for the segment.</span></span> <span data-ttu-id="188d3-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="188d3-118">Read-only.</span></span>|
|<span data-ttu-id="188d3-119">chamador</span><span class="sxs-lookup"><span data-stu-id="188d3-119">caller</span></span>|[<span data-ttu-id="188d3-120">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="188d3-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="188d3-121">Ponto de extremidade que iniciou esse segmento.</span><span class="sxs-lookup"><span data-stu-id="188d3-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="188d3-122">callee</span><span class="sxs-lookup"><span data-stu-id="188d3-122">callee</span></span>|[<span data-ttu-id="188d3-123">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="188d3-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="188d3-124">Ponto de extremidade que respondeu a esse segmento.</span><span class="sxs-lookup"><span data-stu-id="188d3-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="188d3-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="188d3-125">failureInfo</span></span>|[<span data-ttu-id="188d3-126">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="188d3-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="188d3-127">Informações de falha associadas ao segmento se falharem.</span><span class="sxs-lookup"><span data-stu-id="188d3-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="188d3-128">media</span><span class="sxs-lookup"><span data-stu-id="188d3-128">media</span></span>|<span data-ttu-id="188d3-129">[coleção microsoft.graph.callRecords.media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="188d3-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="188d3-130">Mídia associada a esse segmento.</span><span class="sxs-lookup"><span data-stu-id="188d3-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="188d3-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="188d3-131">startDateTime</span></span>|<span data-ttu-id="188d3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="188d3-132">DateTimeOffset</span></span>|<span data-ttu-id="188d3-133">Hora UTC quando o segmento foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="188d3-133">UTC time when the segment started.</span></span> <span data-ttu-id="188d3-134">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="188d3-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="188d3-135">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="188d3-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="188d3-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="188d3-136">endDateTime</span></span>|<span data-ttu-id="188d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="188d3-137">DateTimeOffset</span></span>|<span data-ttu-id="188d3-138">Hora UTC quando o segmento terminou.</span><span class="sxs-lookup"><span data-stu-id="188d3-138">UTC time when the segment ended.</span></span> <span data-ttu-id="188d3-139">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="188d3-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="188d3-140">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="188d3-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="188d3-141">Relações</span><span class="sxs-lookup"><span data-stu-id="188d3-141">Relationships</span></span>

<span data-ttu-id="188d3-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="188d3-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="188d3-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="188d3-143">JSON representation</span></span>

<span data-ttu-id="188d3-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="188d3-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

