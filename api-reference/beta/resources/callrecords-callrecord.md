---
title: tipo de recurso callRecord
description: O tipo callRecord
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 68eeb5fbdf110aa4a8f97c7bf4246897feb22133
ms.sourcegitcommit: 7b1593fc40c910ff7604e9e54577e0c5b8b948dc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2020
ms.locfileid: "44408343"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="77b1e-103">tipo de recurso callRecord</span><span class="sxs-lookup"><span data-stu-id="77b1e-103">callRecord resource type</span></span>

<span data-ttu-id="77b1e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="77b1e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77b1e-105">Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.</span><span class="sxs-lookup"><span data-stu-id="77b1e-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="77b1e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="77b1e-106">Methods</span></span>

| <span data-ttu-id="77b1e-107">Método</span><span class="sxs-lookup"><span data-stu-id="77b1e-107">Method</span></span>       | <span data-ttu-id="77b1e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="77b1e-108">Return Type</span></span> | <span data-ttu-id="77b1e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77b1e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77b1e-110">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="77b1e-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="77b1e-111">Microsoft. Graph. callRecords. callRecord</span><span class="sxs-lookup"><span data-stu-id="77b1e-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="77b1e-112">Leia as propriedades e os relacionamentos do objeto callRecord.</span><span class="sxs-lookup"><span data-stu-id="77b1e-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77b1e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77b1e-113">Properties</span></span>

| <span data-ttu-id="77b1e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77b1e-114">Property</span></span>     | <span data-ttu-id="77b1e-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="77b1e-115">Type</span></span>        | <span data-ttu-id="77b1e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="77b1e-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77b1e-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="77b1e-117">endDateTime</span></span>|<span data-ttu-id="77b1e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77b1e-118">DateTimeOffset</span></span>|<span data-ttu-id="77b1e-119">Hora UTC quando o último usuário saiu da chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="77b1e-120">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="77b1e-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77b1e-121">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="77b1e-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77b1e-122">id</span><span class="sxs-lookup"><span data-stu-id="77b1e-122">id</span></span>|<span data-ttu-id="77b1e-123">String</span><span class="sxs-lookup"><span data-stu-id="77b1e-123">String</span></span>|<span data-ttu-id="77b1e-124">Identificador exclusivo do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-124">Unique identifier for the call record.</span></span> <span data-ttu-id="77b1e-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77b1e-125">Read-only.</span></span>|
|<span data-ttu-id="77b1e-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="77b1e-126">joinWebUrl</span></span>|<span data-ttu-id="77b1e-127">String</span><span class="sxs-lookup"><span data-stu-id="77b1e-127">String</span></span>|<span data-ttu-id="77b1e-128">URL de reunião associada à chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="77b1e-129">Pode não estar disponível para um tipo de registro de chamada peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="77b1e-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="77b1e-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77b1e-130">lastModifiedDateTime</span></span>|<span data-ttu-id="77b1e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77b1e-131">DateTimeOffset</span></span>|<span data-ttu-id="77b1e-132">Hora UTC quando o registro de chamada foi criado.</span><span class="sxs-lookup"><span data-stu-id="77b1e-132">UTC time when the call record was created.</span></span> <span data-ttu-id="77b1e-133">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="77b1e-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77b1e-134">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="77b1e-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77b1e-135">modalidades</span><span class="sxs-lookup"><span data-stu-id="77b1e-135">modalities</span></span>|<span data-ttu-id="77b1e-136">coleção de modalidades de Microsoft. Graph. callRecords.</span><span class="sxs-lookup"><span data-stu-id="77b1e-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="77b1e-137">Lista de todas as modalidades usadas na chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="77b1e-138">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="77b1e-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="77b1e-139">organizer</span><span class="sxs-lookup"><span data-stu-id="77b1e-139">organizer</span></span>|[<span data-ttu-id="77b1e-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="77b1e-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="77b1e-141">A identidade da parte de organização.</span><span class="sxs-lookup"><span data-stu-id="77b1e-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="77b1e-142">participantes</span><span class="sxs-lookup"><span data-stu-id="77b1e-142">participants</span></span>|<span data-ttu-id="77b1e-143">Coleção [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="77b1e-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="77b1e-144">Lista de identidades distintas envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="77b1e-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77b1e-145">startDateTime</span></span>|<span data-ttu-id="77b1e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77b1e-146">DateTimeOffset</span></span>|<span data-ttu-id="77b1e-147">Hora UTC quando o primeiro usuário ingressou na chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="77b1e-148">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="77b1e-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77b1e-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="77b1e-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="77b1e-150">tipo</span><span class="sxs-lookup"><span data-stu-id="77b1e-150">type</span></span>|<span data-ttu-id="77b1e-151">Microsoft. Graph. callRecords. CallType</span><span class="sxs-lookup"><span data-stu-id="77b1e-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="77b1e-152">Indica o tipo da chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-152">Indicates the type of the call.</span></span> <span data-ttu-id="77b1e-153">Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="77b1e-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="77b1e-154">versão</span><span class="sxs-lookup"><span data-stu-id="77b1e-154">version</span></span>|<span data-ttu-id="77b1e-155">Int64</span><span class="sxs-lookup"><span data-stu-id="77b1e-155">Int64</span></span>|<span data-ttu-id="77b1e-156">Versão de aumento monotônico do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="77b1e-157">Registros de chamada de versão superior com a mesma ID incluem dados adicionais comparados à versão inferior.</span><span class="sxs-lookup"><span data-stu-id="77b1e-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77b1e-158">Relações</span><span class="sxs-lookup"><span data-stu-id="77b1e-158">Relationships</span></span>

| <span data-ttu-id="77b1e-159">Relação</span><span class="sxs-lookup"><span data-stu-id="77b1e-159">Relationship</span></span> | <span data-ttu-id="77b1e-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="77b1e-160">Type</span></span>        | <span data-ttu-id="77b1e-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="77b1e-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77b1e-162">sessões</span><span class="sxs-lookup"><span data-stu-id="77b1e-162">sessions</span></span>|<span data-ttu-id="77b1e-163">coleção [Microsoft. Graph. callRecords. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="77b1e-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="77b1e-164">Lista de sessões envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="77b1e-164">List of sessions involved in the call.</span></span> <span data-ttu-id="77b1e-165">As chamadas ponto a ponto normalmente têm apenas uma sessão, enquanto as chamadas de grupo normalmente têm pelo menos uma sessão por participante.</span><span class="sxs-lookup"><span data-stu-id="77b1e-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="77b1e-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77b1e-166">Read-only.</span></span> <span data-ttu-id="77b1e-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="77b1e-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77b1e-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77b1e-168">JSON representation</span></span>

<span data-ttu-id="77b1e-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77b1e-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->