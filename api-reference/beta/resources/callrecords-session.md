---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d72ddd8273088fb7b1401d93e686914a69d18ebd
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394653"
---
# <a name="session-resource-type"></a><span data-ttu-id="b3900-103">tipo de recurso de sessão</span><span class="sxs-lookup"><span data-stu-id="b3900-103">session resource type</span></span>

<span data-ttu-id="b3900-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="b3900-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3900-105">Representa uma comunicação do usuário ou uma comunicação de reunião do usuário no caso de uma chamada em conferência.</span><span class="sxs-lookup"><span data-stu-id="b3900-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="b3900-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b3900-106">Methods</span></span>

<span data-ttu-id="b3900-107">Não existem métodos para acessar diretamente as sessões.</span><span class="sxs-lookup"><span data-stu-id="b3900-107">No methods exist to directly access sessions.</span></span> <span data-ttu-id="b3900-108">Use a API [Get callRecord](../api/callrecords-callrecord-get.md) com `$expand=sessions` para obter as sessões para um [callRecord](callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="b3900-108">Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions` to get the sessions for a [callRecord](callrecords-callrecord.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b3900-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3900-109">Properties</span></span>

| <span data-ttu-id="b3900-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3900-110">Property</span></span>     | <span data-ttu-id="b3900-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3900-111">Type</span></span>        | <span data-ttu-id="b3900-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3900-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3900-113">id</span><span class="sxs-lookup"><span data-stu-id="b3900-113">id</span></span>|<span data-ttu-id="b3900-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3900-114">string</span></span>|<span data-ttu-id="b3900-115">Identificador exclusivo da sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-115">Unique identifier for the session.</span></span> <span data-ttu-id="b3900-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3900-116">Read-only.</span></span>|
|<span data-ttu-id="b3900-117">pelas</span><span class="sxs-lookup"><span data-stu-id="b3900-117">caller</span></span>|[<span data-ttu-id="b3900-118">Microsoft. Graph. callRecords. EndPoint</span><span class="sxs-lookup"><span data-stu-id="b3900-118">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="b3900-119">Ponto de extremidade que iniciou a sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-119">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="b3900-120">receptor</span><span class="sxs-lookup"><span data-stu-id="b3900-120">callee</span></span>|[<span data-ttu-id="b3900-121">Microsoft. Graph. callRecords. EndPoint</span><span class="sxs-lookup"><span data-stu-id="b3900-121">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="b3900-122">Ponto de extremidade que atendeu à sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-122">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="b3900-123">failureInfo</span><span class="sxs-lookup"><span data-stu-id="b3900-123">failureInfo</span></span>|[<span data-ttu-id="b3900-124">Microsoft. Graph. callRecords. failureInfo</span><span class="sxs-lookup"><span data-stu-id="b3900-124">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="b3900-125">Informações de falha associadas à sessão se a sessão falhou.</span><span class="sxs-lookup"><span data-stu-id="b3900-125">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="b3900-126">modalidades</span><span class="sxs-lookup"><span data-stu-id="b3900-126">modalities</span></span>|<span data-ttu-id="b3900-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3900-127">string collection</span></span>|<span data-ttu-id="b3900-128">Lista de modalidades presentes na sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-128">List of modalities present in the session.</span></span> <span data-ttu-id="b3900-129">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b3900-129">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b3900-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b3900-130">startDateTime</span></span>|<span data-ttu-id="b3900-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3900-131">DateTimeOffset</span></span>|<span data-ttu-id="b3900-132">UTC fime quando o primeiro usuário ingressou na sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-132">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="b3900-133">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3900-133">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3900-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b3900-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b3900-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b3900-135">endDateTime</span></span>|<span data-ttu-id="b3900-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3900-136">DateTimeOffset</span></span>|<span data-ttu-id="b3900-137">Hora UTC quando o último usuário saiu da sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-137">UTC time when the last user left the session.</span></span> <span data-ttu-id="b3900-138">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3900-138">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3900-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b3900-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="b3900-140">Relações</span><span class="sxs-lookup"><span data-stu-id="b3900-140">Relationships</span></span>

| <span data-ttu-id="b3900-141">Relação</span><span class="sxs-lookup"><span data-stu-id="b3900-141">Relationship</span></span> | <span data-ttu-id="b3900-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3900-142">Type</span></span>        | <span data-ttu-id="b3900-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3900-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3900-144">segmentos</span><span class="sxs-lookup"><span data-stu-id="b3900-144">segments</span></span>|<span data-ttu-id="b3900-145">coleção [Microsoft. Graph. callRecords. Segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="b3900-145">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="b3900-146">A lista de segmentos envolvidos na sessão.</span><span class="sxs-lookup"><span data-stu-id="b3900-146">The list of segments involved in the session.</span></span> <span data-ttu-id="b3900-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3900-147">Read-only.</span></span> <span data-ttu-id="b3900-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3900-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3900-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3900-149">JSON representation</span></span>

<span data-ttu-id="b3900-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3900-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->