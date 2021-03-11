---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 48983f3a6c4adf12184802722ba2607780c7b531
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720218"
---
# <a name="session-resource-type"></a><span data-ttu-id="7bb1f-103">tipo de recurso de sessão</span><span class="sxs-lookup"><span data-stu-id="7bb1f-103">session resource type</span></span>

<span data-ttu-id="7bb1f-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="7bb1f-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb1f-105">Representa uma User-User ou uma comunicação User-Meeting no caso de uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="7bb1f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7bb1f-106">Methods</span></span>

| <span data-ttu-id="7bb1f-107">Método</span><span class="sxs-lookup"><span data-stu-id="7bb1f-107">Method</span></span>       | <span data-ttu-id="7bb1f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7bb1f-108">Return Type</span></span> | <span data-ttu-id="7bb1f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb1f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7bb1f-110">Listar sessões</span><span class="sxs-lookup"><span data-stu-id="7bb1f-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="7bb1f-111">[coleção microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="7bb1f-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="7bb1f-112">Recupere a lista de sessões associadas a um [objeto callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="7bb1f-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="7bb1f-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bb1f-113">Properties</span></span>

| <span data-ttu-id="7bb1f-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bb1f-114">Property</span></span>     | <span data-ttu-id="7bb1f-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb1f-115">Type</span></span>        | <span data-ttu-id="7bb1f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb1f-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bb1f-117">id</span><span class="sxs-lookup"><span data-stu-id="7bb1f-117">id</span></span>|<span data-ttu-id="7bb1f-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bb1f-118">string</span></span>|<span data-ttu-id="7bb1f-119">Identificador exclusivo da sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-119">Unique identifier for the session.</span></span> <span data-ttu-id="7bb1f-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-120">Read-only.</span></span>|
|<span data-ttu-id="7bb1f-121">chamador</span><span class="sxs-lookup"><span data-stu-id="7bb1f-121">caller</span></span>|[<span data-ttu-id="7bb1f-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="7bb1f-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="7bb1f-123">Ponto de extremidade que iniciou a sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="7bb1f-124">callee</span><span class="sxs-lookup"><span data-stu-id="7bb1f-124">callee</span></span>|[<span data-ttu-id="7bb1f-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="7bb1f-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="7bb1f-126">Ponto de extremidade que atendeu a sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="7bb1f-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="7bb1f-127">failureInfo</span></span>|[<span data-ttu-id="7bb1f-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="7bb1f-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="7bb1f-129">Informações de falha associadas à sessão se a sessão falhou.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="7bb1f-130">modalidades</span><span class="sxs-lookup"><span data-stu-id="7bb1f-130">modalities</span></span>|<span data-ttu-id="7bb1f-131">coleção microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="7bb1f-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="7bb1f-132">Lista de modalidades presentes na sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-132">List of modalities present in the session.</span></span> <span data-ttu-id="7bb1f-133">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7bb1f-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7bb1f-134">startDateTime</span></span>|<span data-ttu-id="7bb1f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bb1f-135">DateTimeOffset</span></span>|<span data-ttu-id="7bb1f-136">FIME UTC quando o primeiro usuário ingressou na sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="7bb1f-137">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7bb1f-138">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="7bb1f-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="7bb1f-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7bb1f-139">endDateTime</span></span>|<span data-ttu-id="7bb1f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bb1f-140">DateTimeOffset</span></span>|<span data-ttu-id="7bb1f-141">Hora UTC quando o último usuário saiu da sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="7bb1f-142">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7bb1f-143">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="7bb1f-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|


## <a name="relationships"></a><span data-ttu-id="7bb1f-144">Relações</span><span class="sxs-lookup"><span data-stu-id="7bb1f-144">Relationships</span></span>

| <span data-ttu-id="7bb1f-145">Relação</span><span class="sxs-lookup"><span data-stu-id="7bb1f-145">Relationship</span></span> | <span data-ttu-id="7bb1f-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb1f-146">Type</span></span>        | <span data-ttu-id="7bb1f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb1f-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bb1f-148">segmentos</span><span class="sxs-lookup"><span data-stu-id="7bb1f-148">segments</span></span>|<span data-ttu-id="7bb1f-149">[coleção microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="7bb1f-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="7bb1f-150">A lista de segmentos envolvidos na sessão.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-150">The list of segments involved in the session.</span></span> <span data-ttu-id="7bb1f-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-151">Read-only.</span></span> <span data-ttu-id="7bb1f-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bb1f-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bb1f-153">JSON representation</span></span>

<span data-ttu-id="7bb1f-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bb1f-154">The following is a JSON representation of the resource.</span></span>

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

