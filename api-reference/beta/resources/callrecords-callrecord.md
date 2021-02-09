---
title: Tipo de recurso callRecord
description: Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 04335e2d804a0d1f824cfc70982e3c138812f8ce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159679"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="5cbeb-103">Tipo de recurso callRecord</span><span class="sxs-lookup"><span data-stu-id="5cbeb-103">callRecord resource type</span></span>

<span data-ttu-id="5cbeb-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="5cbeb-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbeb-105">Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="5cbeb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5cbeb-106">Methods</span></span>

| <span data-ttu-id="5cbeb-107">Método</span><span class="sxs-lookup"><span data-stu-id="5cbeb-107">Method</span></span>       | <span data-ttu-id="5cbeb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5cbeb-108">Return Type</span></span> | <span data-ttu-id="5cbeb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cbeb-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cbeb-110">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="5cbeb-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="5cbeb-111">microsoft.graph.callRecords.callRecord</span><span class="sxs-lookup"><span data-stu-id="5cbeb-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="5cbeb-112">Leia as propriedades e os relacionamentos de um **objeto callRecord.**</span><span class="sxs-lookup"><span data-stu-id="5cbeb-112">Read the properties and relationships of a **callRecord** object.</span></span> |
| [<span data-ttu-id="5cbeb-113">Obter chamadas PSTN</span><span class="sxs-lookup"><span data-stu-id="5cbeb-113">Get PSTN calls</span></span>](../api/callrecords-callrecord-getpstncalls.md) | [<span data-ttu-id="5cbeb-114">microsoft.graph.callRecords.pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="5cbeb-114">microsoft.graph.callRecords.pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)| <span data-ttu-id="5cbeb-115">Leia as propriedades de um **objeto pstnCallLogRow.**</span><span class="sxs-lookup"><span data-stu-id="5cbeb-115">Read the properties of a **pstnCallLogRow** object.</span></span> |
| [<span data-ttu-id="5cbeb-116">Obter chamadas de roteamento direto</span><span class="sxs-lookup"><span data-stu-id="5cbeb-116">Get direct routing calls</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md) | [<span data-ttu-id="5cbeb-117">microsoft.graph.callRecords.directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="5cbeb-117">microsoft.graph.callRecords.directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md)| <span data-ttu-id="5cbeb-118">Leia as propriedades de um **objeto directRoutingLogRow.**</span><span class="sxs-lookup"><span data-stu-id="5cbeb-118">Read the properties of a **directRoutingLogRow** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cbeb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cbeb-119">Properties</span></span>

| <span data-ttu-id="5cbeb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cbeb-120">Property</span></span>     | <span data-ttu-id="5cbeb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cbeb-121">Type</span></span>        | <span data-ttu-id="5cbeb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cbeb-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cbeb-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbeb-123">endDateTime</span></span>|<span data-ttu-id="5cbeb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbeb-124">DateTimeOffset</span></span>|<span data-ttu-id="5cbeb-125">Horário UTC quando o último usuário saiu da chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-125">UTC time when the last user left the call.</span></span> <span data-ttu-id="5cbeb-126">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-126">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cbeb-127">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbeb-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbeb-128">id</span><span class="sxs-lookup"><span data-stu-id="5cbeb-128">id</span></span>|<span data-ttu-id="5cbeb-129">String</span><span class="sxs-lookup"><span data-stu-id="5cbeb-129">String</span></span>|<span data-ttu-id="5cbeb-130">Identificador exclusivo do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-130">Unique identifier for the call record.</span></span> <span data-ttu-id="5cbeb-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-131">Read-only.</span></span>|
|<span data-ttu-id="5cbeb-132">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="5cbeb-132">joinWebUrl</span></span>|<span data-ttu-id="5cbeb-133">String</span><span class="sxs-lookup"><span data-stu-id="5cbeb-133">String</span></span>|<span data-ttu-id="5cbeb-134">URL de reunião associada à chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-134">Meeting URL associated to the call.</span></span> <span data-ttu-id="5cbeb-135">Pode não estar disponível para um tipo de registro de chamada peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-135">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="5cbeb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbeb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5cbeb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbeb-137">DateTimeOffset</span></span>|<span data-ttu-id="5cbeb-138">Hora UTC em que o registro de chamada foi criado.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-138">UTC time when the call record was created.</span></span> <span data-ttu-id="5cbeb-139">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-139">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cbeb-140">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbeb-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbeb-141">modalidades</span><span class="sxs-lookup"><span data-stu-id="5cbeb-141">modalities</span></span>|<span data-ttu-id="5cbeb-142">coleção microsoft.graph.callRecords.modality</span><span class="sxs-lookup"><span data-stu-id="5cbeb-142">microsoft.graph.callRecords.modality collection</span></span>|<span data-ttu-id="5cbeb-143">Lista de todas as modalidades usadas na chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-143">List of all the modalities used in the call.</span></span> <span data-ttu-id="5cbeb-144">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-144">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5cbeb-145">organizer</span><span class="sxs-lookup"><span data-stu-id="5cbeb-145">organizer</span></span>|[<span data-ttu-id="5cbeb-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="5cbeb-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="5cbeb-147">A identidade da organização.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-147">The organizing party's identity.</span></span>|
|<span data-ttu-id="5cbeb-148">participantes</span><span class="sxs-lookup"><span data-stu-id="5cbeb-148">participants</span></span>|<span data-ttu-id="5cbeb-149">Coleção [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="5cbeb-149">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="5cbeb-150">Lista de identidades distintas envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-150">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="5cbeb-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbeb-151">startDateTime</span></span>|<span data-ttu-id="5cbeb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbeb-152">DateTimeOffset</span></span>|<span data-ttu-id="5cbeb-153">Horário UTC quando o primeiro usuário ingressou na chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-153">UTC time when the first user joined the call.</span></span> <span data-ttu-id="5cbeb-154">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-154">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cbeb-155">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbeb-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbeb-156">type</span><span class="sxs-lookup"><span data-stu-id="5cbeb-156">type</span></span>|<span data-ttu-id="5cbeb-157">microsoft.graph.callRecords.callType</span><span class="sxs-lookup"><span data-stu-id="5cbeb-157">microsoft.graph.callRecords.callType</span></span>|<span data-ttu-id="5cbeb-158">Indica o tipo da chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-158">Indicates the type of the call.</span></span> <span data-ttu-id="5cbeb-159">Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-159">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5cbeb-160">versão</span><span class="sxs-lookup"><span data-stu-id="5cbeb-160">version</span></span>|<span data-ttu-id="5cbeb-161">Int64</span><span class="sxs-lookup"><span data-stu-id="5cbeb-161">Int64</span></span>|<span data-ttu-id="5cbeb-162">Versão crescente monotônica do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-162">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="5cbeb-163">Registros de chamada de versão superior com a mesma ID incluem dados adicionais em comparação com a versão inferior.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-163">Higher version call records with the same ID includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cbeb-164">Relações</span><span class="sxs-lookup"><span data-stu-id="5cbeb-164">Relationships</span></span>

| <span data-ttu-id="5cbeb-165">Relação</span><span class="sxs-lookup"><span data-stu-id="5cbeb-165">Relationship</span></span> | <span data-ttu-id="5cbeb-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cbeb-166">Type</span></span>        | <span data-ttu-id="5cbeb-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cbeb-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cbeb-168">sessões</span><span class="sxs-lookup"><span data-stu-id="5cbeb-168">sessions</span></span>|<span data-ttu-id="5cbeb-169">[coleção microsoft.graph.callRecords.session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="5cbeb-169">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="5cbeb-170">Lista de sessões envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-170">List of sessions involved in the call.</span></span> <span data-ttu-id="5cbeb-171">Chamadas ponto a ponto geralmente têm apenas uma sessão, enquanto chamadas de grupo geralmente têm pelo menos uma sessão por participante.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-171">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="5cbeb-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-172">Read-only.</span></span> <span data-ttu-id="5cbeb-173">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-173">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cbeb-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cbeb-174">JSON representation</span></span>

<span data-ttu-id="5cbeb-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cbeb-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
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


