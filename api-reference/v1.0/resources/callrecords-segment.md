---
title: tipo de recurso Segment
description: O tipo de segmento
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6c38dac3d0e2e30c8b90e9fb0029d463b700f124
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491943"
---
# <a name="segment-resource-type"></a><span data-ttu-id="63f7e-103">tipo de recurso Segment</span><span class="sxs-lookup"><span data-stu-id="63f7e-103">segment resource type</span></span>

<span data-ttu-id="63f7e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="63f7e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="63f7e-105">Representa uma parte de uma comunicação do usuário ou uma comunicação de reunião do usuário no caso de uma chamada em conferência.</span><span class="sxs-lookup"><span data-stu-id="63f7e-105">Represents a portion of a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span> <span data-ttu-id="63f7e-106">Uma chamada VOIP típica terá um segmento por sessão.</span><span class="sxs-lookup"><span data-stu-id="63f7e-106">A typical VOIP call will have one segment per session.</span></span> <span data-ttu-id="63f7e-107">Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão, devido à comunicação adicional de servidor para servidor necessária para conectar a chamada.</span><span class="sxs-lookup"><span data-stu-id="63f7e-107">In certain scenarios, such as PSTN calls, there will be multiple segments per session due to additional server-to-server communication required to connect the call.</span></span>

## <a name="methods"></a><span data-ttu-id="63f7e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="63f7e-108">Methods</span></span>

<span data-ttu-id="63f7e-109">Não existem métodos para acessar diretamente os segmentos.</span><span class="sxs-lookup"><span data-stu-id="63f7e-109">No methods exist to directly access segments.</span></span> <span data-ttu-id="63f7e-110">Use a API [Get callRecord](../api/callrecords-callrecord-get.md) com `$expand=sessions($expand=segments)` ou a API de [sessão de lista](../api/callrecords-session-list.md) com `$expand=segments` para obter os segmentos de um [callRecord](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="63f7e-110">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the [List session](../api/callrecords-session-list.md) api with `$expand=segments` to get the segments for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="63f7e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63f7e-111">Properties</span></span>

| <span data-ttu-id="63f7e-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63f7e-112">Property</span></span>     | <span data-ttu-id="63f7e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f7e-113">Type</span></span>        | <span data-ttu-id="63f7e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f7e-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63f7e-115">id</span><span class="sxs-lookup"><span data-stu-id="63f7e-115">id</span></span>|<span data-ttu-id="63f7e-116">String</span><span class="sxs-lookup"><span data-stu-id="63f7e-116">String</span></span>|<span data-ttu-id="63f7e-117">Identificador exclusivo do segmento.</span><span class="sxs-lookup"><span data-stu-id="63f7e-117">Unique identifier for the segment.</span></span> <span data-ttu-id="63f7e-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63f7e-118">Read-only.</span></span>|
|<span data-ttu-id="63f7e-119">pelas</span><span class="sxs-lookup"><span data-stu-id="63f7e-119">caller</span></span>|[<span data-ttu-id="63f7e-120">Microsoft. Graph. callRecords. EndPoint</span><span class="sxs-lookup"><span data-stu-id="63f7e-120">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="63f7e-121">Ponto de extremidade que iniciou este segmento.</span><span class="sxs-lookup"><span data-stu-id="63f7e-121">Endpoint that initiated this segment.</span></span>|
|<span data-ttu-id="63f7e-122">receptor</span><span class="sxs-lookup"><span data-stu-id="63f7e-122">callee</span></span>|[<span data-ttu-id="63f7e-123">Microsoft. Graph. callRecords. EndPoint</span><span class="sxs-lookup"><span data-stu-id="63f7e-123">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="63f7e-124">Ponto de extremidade que respondeu a este segmento.</span><span class="sxs-lookup"><span data-stu-id="63f7e-124">Endpoint that answered this segment.</span></span>|
|<span data-ttu-id="63f7e-125">failureInfo</span><span class="sxs-lookup"><span data-stu-id="63f7e-125">failureInfo</span></span>|[<span data-ttu-id="63f7e-126">Microsoft. Graph. callRecords. failureInfo</span><span class="sxs-lookup"><span data-stu-id="63f7e-126">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="63f7e-127">Informações de falha associadas ao segmento se ele falhar.</span><span class="sxs-lookup"><span data-stu-id="63f7e-127">Failure information associated with the segment if it failed.</span></span>|
|<span data-ttu-id="63f7e-128">corre</span><span class="sxs-lookup"><span data-stu-id="63f7e-128">media</span></span>|<span data-ttu-id="63f7e-129">coleção [Microsoft. Graph. callRecords. Media](callrecords-media.md)</span><span class="sxs-lookup"><span data-stu-id="63f7e-129">[microsoft.graph.callRecords.media](callrecords-media.md) collection</span></span>|<span data-ttu-id="63f7e-130">Mídia associada a este segmento.</span><span class="sxs-lookup"><span data-stu-id="63f7e-130">Media associated with this segment.</span></span>|
|<span data-ttu-id="63f7e-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="63f7e-131">startDateTime</span></span>|<span data-ttu-id="63f7e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63f7e-132">DateTimeOffset</span></span>|<span data-ttu-id="63f7e-133">Hora UTC quando o segmento é iniciado.</span><span class="sxs-lookup"><span data-stu-id="63f7e-133">UTC time when the segment started.</span></span> <span data-ttu-id="63f7e-134">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="63f7e-134">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="63f7e-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="63f7e-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="63f7e-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="63f7e-136">endDateTime</span></span>|<span data-ttu-id="63f7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63f7e-137">DateTimeOffset</span></span>|<span data-ttu-id="63f7e-138">Hora UTC em que o segmento terminou.</span><span class="sxs-lookup"><span data-stu-id="63f7e-138">UTC time when the segment ended.</span></span> <span data-ttu-id="63f7e-139">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="63f7e-139">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="63f7e-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="63f7e-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="63f7e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="63f7e-141">Relationships</span></span>

<span data-ttu-id="63f7e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63f7e-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63f7e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63f7e-143">JSON representation</span></span>

<span data-ttu-id="63f7e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63f7e-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
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