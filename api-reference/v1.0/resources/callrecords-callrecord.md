---
title: tipo de recurso callRecord
description: O tipo callRecord
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dbc0884ad03be4186d5a08c59e4494413b0b1a29
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988461"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="bfcfb-103">tipo de recurso callRecord</span><span class="sxs-lookup"><span data-stu-id="bfcfb-103">callRecord resource type</span></span>

<span data-ttu-id="bfcfb-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="bfcfb-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="bfcfb-105">Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="bfcfb-106">Methods</span><span class="sxs-lookup"><span data-stu-id="bfcfb-106">Methods</span></span>

| <span data-ttu-id="bfcfb-107">Método</span><span class="sxs-lookup"><span data-stu-id="bfcfb-107">Method</span></span>       | <span data-ttu-id="bfcfb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfcfb-108">Return Type</span></span> | <span data-ttu-id="bfcfb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcfb-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bfcfb-110">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="bfcfb-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="bfcfb-111">Microsoft. Graph. callRecords. callRecord</span><span class="sxs-lookup"><span data-stu-id="bfcfb-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="bfcfb-112">Leia as propriedades e os relacionamentos do objeto callRecord.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-112">Read properties and relationships of callRecord object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfcfb-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfcfb-113">Properties</span></span>

| <span data-ttu-id="bfcfb-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfcfb-114">Property</span></span>     | <span data-ttu-id="bfcfb-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfcfb-115">Type</span></span>        | <span data-ttu-id="bfcfb-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcfb-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfcfb-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bfcfb-117">endDateTime</span></span>|<span data-ttu-id="bfcfb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfcfb-118">DateTimeOffset</span></span>|<span data-ttu-id="bfcfb-119">Hora UTC quando o último usuário saiu da chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="bfcfb-120">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfcfb-121">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfcfb-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfcfb-122">id</span><span class="sxs-lookup"><span data-stu-id="bfcfb-122">id</span></span>|<span data-ttu-id="bfcfb-123">String</span><span class="sxs-lookup"><span data-stu-id="bfcfb-123">String</span></span>|<span data-ttu-id="bfcfb-124">Identificador exclusivo do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-124">Unique identifier for the call record.</span></span> <span data-ttu-id="bfcfb-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-125">Read-only.</span></span>|
|<span data-ttu-id="bfcfb-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="bfcfb-126">joinWebUrl</span></span>|<span data-ttu-id="bfcfb-127">String</span><span class="sxs-lookup"><span data-stu-id="bfcfb-127">String</span></span>|<span data-ttu-id="bfcfb-128">URL de reunião associada à chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="bfcfb-129">Pode não estar disponível para um tipo de registro de chamada peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="bfcfb-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfcfb-130">lastModifiedDateTime</span></span>|<span data-ttu-id="bfcfb-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfcfb-131">DateTimeOffset</span></span>|<span data-ttu-id="bfcfb-132">Hora UTC quando o registro de chamada foi criado.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-132">UTC time when the call record was created.</span></span> <span data-ttu-id="bfcfb-133">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfcfb-134">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfcfb-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfcfb-135">modalidades</span><span class="sxs-lookup"><span data-stu-id="bfcfb-135">modalities</span></span>|<span data-ttu-id="bfcfb-136">coleção de modalidades de Microsoft. Graph. callRecords.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-136">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="bfcfb-137">Lista de todas as modalidades usadas na chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="bfcfb-138">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bfcfb-139">organizer</span><span class="sxs-lookup"><span data-stu-id="bfcfb-139">organizer</span></span>|[<span data-ttu-id="bfcfb-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="bfcfb-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="bfcfb-141">A identidade da parte de organização.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="bfcfb-142">participantes</span><span class="sxs-lookup"><span data-stu-id="bfcfb-142">participants</span></span>|<span data-ttu-id="bfcfb-143">Coleção [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="bfcfb-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="bfcfb-144">Lista de identidades distintas envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="bfcfb-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bfcfb-145">startDateTime</span></span>|<span data-ttu-id="bfcfb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfcfb-146">DateTimeOffset</span></span>|<span data-ttu-id="bfcfb-147">Hora UTC quando o primeiro usuário ingressou na chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="bfcfb-148">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfcfb-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfcfb-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfcfb-150">tipo</span><span class="sxs-lookup"><span data-stu-id="bfcfb-150">type</span></span>|<span data-ttu-id="bfcfb-151">Microsoft. Graph. callRecords. CallType</span><span class="sxs-lookup"><span data-stu-id="bfcfb-151">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="bfcfb-152">Indica o tipo da chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-152">Indicates the type of the call.</span></span> <span data-ttu-id="bfcfb-153">Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bfcfb-154">versão</span><span class="sxs-lookup"><span data-stu-id="bfcfb-154">version</span></span>|<span data-ttu-id="bfcfb-155">Int64</span><span class="sxs-lookup"><span data-stu-id="bfcfb-155">Int64</span></span>|<span data-ttu-id="bfcfb-156">Versão de aumento monotônico do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="bfcfb-157">Registros de chamada de versão superior com a mesma ID incluem dados adicionais comparados à versão inferior.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfcfb-158">Relações</span><span class="sxs-lookup"><span data-stu-id="bfcfb-158">Relationships</span></span>

| <span data-ttu-id="bfcfb-159">Relação</span><span class="sxs-lookup"><span data-stu-id="bfcfb-159">Relationship</span></span> | <span data-ttu-id="bfcfb-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfcfb-160">Type</span></span>        | <span data-ttu-id="bfcfb-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcfb-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfcfb-162">sessões</span><span class="sxs-lookup"><span data-stu-id="bfcfb-162">sessions</span></span>|<span data-ttu-id="bfcfb-163">coleção [Microsoft. Graph. callRecords. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="bfcfb-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="bfcfb-164">Lista de sessões envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-164">List of sessions involved in the call.</span></span> <span data-ttu-id="bfcfb-165">As chamadas ponto a ponto normalmente têm apenas uma sessão, enquanto as chamadas de grupo normalmente têm pelo menos uma sessão por participante.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="bfcfb-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-166">Read-only.</span></span> <span data-ttu-id="bfcfb-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfcfb-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfcfb-168">JSON representation</span></span>

<span data-ttu-id="bfcfb-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfcfb-169">The following is a JSON representation of the resource.</span></span>

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
