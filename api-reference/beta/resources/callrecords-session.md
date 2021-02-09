---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 263ad4d249535fc9255507e398b29d69b34bbb7d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155570"
---
# <a name="session-resource-type"></a><span data-ttu-id="bbf26-103">tipo de recurso de sessão</span><span class="sxs-lookup"><span data-stu-id="bbf26-103">session resource type</span></span>

<span data-ttu-id="bbf26-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bbf26-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf26-105">Representa uma User-User comunicação ou uma User-Meeting no caso de uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="bbf26-105">Represents a User-User communication or a User-Meeting communication in the case of a Conference call.</span></span>

## <a name="methods"></a><span data-ttu-id="bbf26-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bbf26-106">Methods</span></span>

| <span data-ttu-id="bbf26-107">Método</span><span class="sxs-lookup"><span data-stu-id="bbf26-107">Method</span></span>       | <span data-ttu-id="bbf26-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bbf26-108">Return Type</span></span> | <span data-ttu-id="bbf26-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf26-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bbf26-110">Listar sessões</span><span class="sxs-lookup"><span data-stu-id="bbf26-110">List sessions</span></span>](../api/callrecords-session-list.md) | <span data-ttu-id="bbf26-111">[coleção microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="bbf26-111">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span> | <span data-ttu-id="bbf26-112">Recupere a lista de sessões associadas a um [objeto callRecord.](callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="bbf26-112">Retrieve the list of sessions associated with a [callRecord](callrecords-callrecord.md) object.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="bbf26-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbf26-113">Properties</span></span>

| <span data-ttu-id="bbf26-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbf26-114">Property</span></span>     | <span data-ttu-id="bbf26-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf26-115">Type</span></span>        | <span data-ttu-id="bbf26-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf26-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbf26-117">id</span><span class="sxs-lookup"><span data-stu-id="bbf26-117">id</span></span>|<span data-ttu-id="bbf26-118">string</span><span class="sxs-lookup"><span data-stu-id="bbf26-118">string</span></span>|<span data-ttu-id="bbf26-119">Identificador exclusivo da sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-119">Unique identifier for the session.</span></span> <span data-ttu-id="bbf26-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bbf26-120">Read-only.</span></span>|
|<span data-ttu-id="bbf26-121">chamador</span><span class="sxs-lookup"><span data-stu-id="bbf26-121">caller</span></span>|[<span data-ttu-id="bbf26-122">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="bbf26-122">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="bbf26-123">Ponto de extremidade que iniciou a sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-123">Endpoint that initiated the session.</span></span>|
|<span data-ttu-id="bbf26-124">destinatário da chamada</span><span class="sxs-lookup"><span data-stu-id="bbf26-124">callee</span></span>|[<span data-ttu-id="bbf26-125">microsoft.graph.callRecords.endpoint</span><span class="sxs-lookup"><span data-stu-id="bbf26-125">microsoft.graph.callRecords.endpoint</span></span>](callrecords-endpoint.md)|<span data-ttu-id="bbf26-126">Ponto de extremidade que atendeu a sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-126">Endpoint that answered the session.</span></span>|
|<span data-ttu-id="bbf26-127">failureInfo</span><span class="sxs-lookup"><span data-stu-id="bbf26-127">failureInfo</span></span>|[<span data-ttu-id="bbf26-128">microsoft.graph.callRecords.failureInfo</span><span class="sxs-lookup"><span data-stu-id="bbf26-128">microsoft.graph.callRecords.failureInfo</span></span>](callrecords-failureinfo.md)|<span data-ttu-id="bbf26-129">Informações de falha associadas à sessão se a sessão falhou.</span><span class="sxs-lookup"><span data-stu-id="bbf26-129">Failure information associated with the session if the session failed.</span></span>|
|<span data-ttu-id="bbf26-130">modalidades</span><span class="sxs-lookup"><span data-stu-id="bbf26-130">modalities</span></span>|<span data-ttu-id="bbf26-131">coleção microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="bbf26-131">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="bbf26-132">Lista de modalidades presentes na sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-132">List of modalities present in the session.</span></span> <span data-ttu-id="bbf26-133">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bbf26-133">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bbf26-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf26-134">startDateTime</span></span>|<span data-ttu-id="bbf26-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf26-135">DateTimeOffset</span></span>|<span data-ttu-id="bbf26-136">FIME UTC quando o primeiro usuário ingressou na sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-136">UTC fime when the first user joined the session.</span></span> <span data-ttu-id="bbf26-137">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bbf26-137">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbf26-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bbf26-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bbf26-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf26-139">endDateTime</span></span>|<span data-ttu-id="bbf26-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf26-140">DateTimeOffset</span></span>|<span data-ttu-id="bbf26-141">Horário UTC quando o último usuário saiu da sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-141">UTC time when the last user left the session.</span></span> <span data-ttu-id="bbf26-142">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bbf26-142">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbf26-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bbf26-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|


## <a name="relationships"></a><span data-ttu-id="bbf26-144">Relações</span><span class="sxs-lookup"><span data-stu-id="bbf26-144">Relationships</span></span>

| <span data-ttu-id="bbf26-145">Relação</span><span class="sxs-lookup"><span data-stu-id="bbf26-145">Relationship</span></span> | <span data-ttu-id="bbf26-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf26-146">Type</span></span>        | <span data-ttu-id="bbf26-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf26-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbf26-148">segmentos</span><span class="sxs-lookup"><span data-stu-id="bbf26-148">segments</span></span>|<span data-ttu-id="bbf26-149">[coleção microsoft.graph.callRecords.segment](callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="bbf26-149">[microsoft.graph.callRecords.segment](callrecords-segment.md) collection</span></span>|<span data-ttu-id="bbf26-150">A lista de segmentos envolvidos na sessão.</span><span class="sxs-lookup"><span data-stu-id="bbf26-150">The list of segments involved in the session.</span></span> <span data-ttu-id="bbf26-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bbf26-151">Read-only.</span></span> <span data-ttu-id="bbf26-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bbf26-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbf26-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbf26-153">JSON representation</span></span>

<span data-ttu-id="bbf26-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbf26-154">The following is a JSON representation of the resource.</span></span>

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

