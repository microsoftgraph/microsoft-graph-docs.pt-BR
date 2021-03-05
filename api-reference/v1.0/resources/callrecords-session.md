---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: db45e2a7ed1103e03a22b5f06e16abc6541aec81
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434248"
---
# <a name="session-resource-type"></a><span data-ttu-id="e08fc-103">tipo de recurso de sessão</span><span class="sxs-lookup"><span data-stu-id="e08fc-103">session resource type</span></span>

<span data-ttu-id="e08fc-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e08fc-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="e08fc-105">Representa uma User-User ou uma comunicação User-Meeting no caso de uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="e08fc-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="e08fc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e08fc-106">Methods</span></span>

| <span data-ttu-id="e08fc-107">Método</span><span class="sxs-lookup"><span data-stu-id="e08fc-107">Method</span></span>       | <span data-ttu-id="e08fc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e08fc-108">Return Type</span></span> | <span data-ttu-id="e08fc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08fc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e08fc-110">Listar sessões</span><span class="sxs-lookup"><span data-stu-id="e08fc-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="e08fc-111">[coleção microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="e08fc-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="e08fc-112">Recupere a lista de sessões associadas a um [objeto callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="e08fc-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="e08fc-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e08fc-113">Properties</span></span>

| <span data-ttu-id="e08fc-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e08fc-114">Property</span></span>     | <span data-ttu-id="e08fc-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e08fc-115">Type</span></span>        | <span data-ttu-id="e08fc-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08fc-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e08fc-117">id</span><span class="sxs-lookup"><span data-stu-id="e08fc-117">id</span></span>|<span data-ttu-id="e08fc-118">string</span><span class="sxs-lookup"><span data-stu-id="e08fc-118">string</span></span>|<span data-ttu-id="e08fc-119">Identificador exclusivo da sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-119">Unique identifier for the session.</span></span> <span data-ttu-id="e08fc-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e08fc-120">Read-only.</span></span>|
|<span data-ttu-id="e08fc-121">chamador</span><span class="sxs-lookup"><span data-stu-id="e08fc-121">caller</span></span>|[<span data-ttu-id="e08fc-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="e08fc-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e08fc-123">Ponto de extremidade que iniciou a sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="e08fc-124">callee</span><span class="sxs-lookup"><span data-stu-id="e08fc-124">callee</span></span>|[<span data-ttu-id="e08fc-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="e08fc-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="e08fc-126">Ponto de extremidade que atendeu a sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="e08fc-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="e08fc-127">failureInfo</span></span>|[<span data-ttu-id="e08fc-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="e08fc-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="e08fc-129">Informações de falha associadas à sessão se a sessão falhou.</span><span class="sxs-lookup"><span data-stu-id="e08fc-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="e08fc-130">modalidades</span><span class="sxs-lookup"><span data-stu-id="e08fc-130">modalities</span></span>|<span data-ttu-id="e08fc-131">coleção microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="e08fc-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="e08fc-132">Lista de modalidades presentes na sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-132">List of modalities present in the session.</span></span> <span data-ttu-id="e08fc-133">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e08fc-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e08fc-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e08fc-134">startDateTime</span></span>|<span data-ttu-id="e08fc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e08fc-135">DateTimeOffset</span></span>|<span data-ttu-id="e08fc-136">Hora UTC quando o primeiro usuário ingressou na sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-136">UTC time when the first user joined the session.</span></span> <span data-ttu-id="e08fc-137">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e08fc-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e08fc-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e08fc-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e08fc-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e08fc-139">endDateTime</span></span>|<span data-ttu-id="e08fc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e08fc-140">DateTimeOffset</span></span>|<span data-ttu-id="e08fc-141">Hora UTC quando o último usuário saiu da sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="e08fc-142">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e08fc-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e08fc-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e08fc-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="e08fc-144">Relações</span><span class="sxs-lookup"><span data-stu-id="e08fc-144">Relationships</span></span>

| <span data-ttu-id="e08fc-145">Relação</span><span class="sxs-lookup"><span data-stu-id="e08fc-145">Relationship</span></span> | <span data-ttu-id="e08fc-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="e08fc-146">Type</span></span>        | <span data-ttu-id="e08fc-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08fc-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e08fc-148">segmentos</span><span class="sxs-lookup"><span data-stu-id="e08fc-148">segments</span></span>|<span data-ttu-id="e08fc-149">[coleção microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="e08fc-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="e08fc-150">A lista de segmentos envolvidos na sessão.</span><span class="sxs-lookup"><span data-stu-id="e08fc-150">The list of segments involved in the session.</span></span> <span data-ttu-id="e08fc-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e08fc-151">Read-only.</span></span> <span data-ttu-id="e08fc-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e08fc-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e08fc-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e08fc-153">JSON representation</span></span>

<span data-ttu-id="e08fc-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e08fc-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
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
