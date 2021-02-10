---
title: tipo de recurso segment
description: O tipo de segmento
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9240e0189bd9cc8a7961894562cdc9178ba07893
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153470"
---
# <a name="segment-resource-type"></a><span data-ttu-id="20cff-103">tipo de recurso segment</span><span class="sxs-lookup"><span data-stu-id="20cff-103">segment resource type</span></span>

<span data-ttu-id="20cff-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="20cff-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="20cff-105">Representa uma parte de uma User-User comunicação ou uma User-Meeting no caso de uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="20cff-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="20cff-106">Uma chamada VOIP típica terá um segmento por sessão.</span><span class="sxs-lookup"><span data-stu-id="20cff-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="20cff-107">Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão devido à comunicação adicional entre servidores necessária para conectar a chamada.</span><span class="sxs-lookup"><span data-stu-id="20cff-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="20cff-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="20cff-108">Methods</span></span>

<span data-ttu-id="20cff-109">Não existem métodos para acessar diretamente segmentos.</span><span class="sxs-lookup"><span data-stu-id="20cff-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="20cff-110">Use a api [Obter callRecord](../api/callrecords-callrecord-get.md) com ou a api de sessão de lista com para `$expand=sessions($expand=segments)` obter os [](../api/callrecords-session-list.md) `$expand=segments` segmentos de um [callRecord](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="20cff-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20cff-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20cff-111">Properties</span></span>

| <span data-ttu-id="20cff-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20cff-112">Property</span></span>     | <span data-ttu-id="20cff-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="20cff-113">Type</span></span>        | <span data-ttu-id="20cff-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="20cff-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20cff-115">id</span><span class="sxs-lookup"><span data-stu-id="20cff-115">id</span></span>|<span data-ttu-id="20cff-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20cff-116">String</span></span>|<span data-ttu-id="20cff-117">Identificador exclusivo do segmento.</span><span class="sxs-lookup"><span data-stu-id="20cff-117">Unique identifier for the segment.</span></span> <span data-ttu-id="20cff-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20cff-118">Read-only.</span></span>|
|<span data-ttu-id="20cff-119">chamador</span><span class="sxs-lookup"><span data-stu-id="20cff-119">caller</span></span>|[<span data-ttu-id="20cff-120">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="20cff-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="20cff-121">Ponto de extremidade que iniciou esse segmento.</span><span class="sxs-lookup"><span data-stu-id="20cff-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="20cff-122">destinatário da chamada</span><span class="sxs-lookup"><span data-stu-id="20cff-122">callee</span></span>|[<span data-ttu-id="20cff-123">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="20cff-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="20cff-124">Ponto de extremidade que atendeu esse segmento.</span><span class="sxs-lookup"><span data-stu-id="20cff-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="20cff-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="20cff-125">failureInfo</span></span>|[<span data-ttu-id="20cff-126">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="20cff-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="20cff-127">Informações de falha associadas ao segmento em caso de falha.</span><span class="sxs-lookup"><span data-stu-id="20cff-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="20cff-128">mídia</span><span class="sxs-lookup"><span data-stu-id="20cff-128">media</span></span>|<span data-ttu-id="20cff-129">[coleção microsoft.graph.callRecords.media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="20cff-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="20cff-130">Mídia associada a este segmento.</span><span class="sxs-lookup"><span data-stu-id="20cff-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="20cff-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20cff-131">startDateTime</span></span>|<span data-ttu-id="20cff-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20cff-132">DateTimeOffset</span></span>|<span data-ttu-id="20cff-133">Horário UTC quando o segmento foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="20cff-133">UTC time when the segment started.</span></span> <span data-ttu-id="20cff-134">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="20cff-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="20cff-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="20cff-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="20cff-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="20cff-136">endDateTime</span></span>|<span data-ttu-id="20cff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20cff-137">DateTimeOffset</span></span>|<span data-ttu-id="20cff-138">Hora UTC quando o segmento terminou.</span><span class="sxs-lookup"><span data-stu-id="20cff-138">UTC time when the segment ended.</span></span> <span data-ttu-id="20cff-139">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="20cff-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="20cff-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="20cff-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="20cff-141">Relações</span><span class="sxs-lookup"><span data-stu-id="20cff-141">Relationships</span></span>

<span data-ttu-id="20cff-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20cff-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20cff-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20cff-143">JSON representation</span></span>

<span data-ttu-id="20cff-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20cff-144">The following is a JSON representation of the resource.</span></span>

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
