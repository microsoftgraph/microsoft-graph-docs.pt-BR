---
title: tipo de recurso callRecord
description: O tipo callRecord
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0eddc25f92c7043425ff63c46ce5fbba23f5a1be
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394703"
---
# <a name="callrecord-resource-type"></a><span data-ttu-id="8953b-103">tipo de recurso callRecord</span><span class="sxs-lookup"><span data-stu-id="8953b-103">callRecord resource type</span></span>

<span data-ttu-id="8953b-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="8953b-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8953b-105">Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.</span><span class="sxs-lookup"><span data-stu-id="8953b-105">Represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="8953b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8953b-106">Methods</span></span>

| <span data-ttu-id="8953b-107">Método</span><span class="sxs-lookup"><span data-stu-id="8953b-107">Method</span></span>       | <span data-ttu-id="8953b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8953b-108">Return Type</span></span> | <span data-ttu-id="8953b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8953b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8953b-110">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="8953b-110">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) | [<span data-ttu-id="8953b-111">Microsoft. Graph. callRecords. callRecord</span><span class="sxs-lookup"><span data-stu-id="8953b-111">microsoft.graph.callRecords.callRecord</span></span>](callrecords-callrecord.md) | <span data-ttu-id="8953b-112">Leia as propriedades e os relacionamentos do objeto callRecord.</span><span class="sxs-lookup"><span data-stu-id="8953b-112">Read properties and relationships of callRecord object.</span></span> |
## <a name="properties"></a><span data-ttu-id="8953b-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8953b-113">Properties</span></span>

| <span data-ttu-id="8953b-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8953b-114">Property</span></span>     | <span data-ttu-id="8953b-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="8953b-115">Type</span></span>        | <span data-ttu-id="8953b-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8953b-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8953b-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8953b-117">endDateTime</span></span>|<span data-ttu-id="8953b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8953b-118">DateTimeOffset</span></span>|<span data-ttu-id="8953b-119">Hora UTC quando o último usuário saiu da chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-119">UTC time when the last user left the call.</span></span> <span data-ttu-id="8953b-120">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8953b-120">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8953b-121">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8953b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8953b-122">id</span><span class="sxs-lookup"><span data-stu-id="8953b-122">id</span></span>|<span data-ttu-id="8953b-123">String</span><span class="sxs-lookup"><span data-stu-id="8953b-123">String</span></span>|<span data-ttu-id="8953b-124">Identificador exclusivo do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-124">Unique identifier for the call record.</span></span> <span data-ttu-id="8953b-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8953b-125">Read-only.</span></span>|
|<span data-ttu-id="8953b-126">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="8953b-126">joinWebUrl</span></span>|<span data-ttu-id="8953b-127">String</span><span class="sxs-lookup"><span data-stu-id="8953b-127">String</span></span>|<span data-ttu-id="8953b-128">URL de reunião associada à chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-128">Meeting URL associated to the call.</span></span> <span data-ttu-id="8953b-129">Pode não estar disponível para um tipo de registro de chamada peerToPeer.</span><span class="sxs-lookup"><span data-stu-id="8953b-129">May not be available for a peerToPeer call record type.</span></span>|
|<span data-ttu-id="8953b-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8953b-130">lastModifiedDateTime</span></span>|<span data-ttu-id="8953b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8953b-131">DateTimeOffset</span></span>|<span data-ttu-id="8953b-132">Hora UTC quando o registro de chamada foi criado.</span><span class="sxs-lookup"><span data-stu-id="8953b-132">UTC time when the call record was created.</span></span> <span data-ttu-id="8953b-133">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8953b-133">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8953b-134">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8953b-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8953b-135">modalidades</span><span class="sxs-lookup"><span data-stu-id="8953b-135">modalities</span></span>|<span data-ttu-id="8953b-136">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8953b-136">string collection</span></span>|<span data-ttu-id="8953b-137">Lista de todas as modalidades usadas na chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-137">List of all the modalities used in the call.</span></span> <span data-ttu-id="8953b-138">Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8953b-138">Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8953b-139">organizer</span><span class="sxs-lookup"><span data-stu-id="8953b-139">organizer</span></span>|[<span data-ttu-id="8953b-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="8953b-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="8953b-141">A identidade da parte de organização.</span><span class="sxs-lookup"><span data-stu-id="8953b-141">The organizing party's identity.</span></span>|
|<span data-ttu-id="8953b-142">participantes</span><span class="sxs-lookup"><span data-stu-id="8953b-142">participants</span></span>|<span data-ttu-id="8953b-143">Coleção [identitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="8953b-143">[identitySet](identityset.md) collection</span></span>|<span data-ttu-id="8953b-144">Lista de identidades distintas envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-144">List of distinct identities involved in the call.</span></span>|
|<span data-ttu-id="8953b-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8953b-145">startDateTime</span></span>|<span data-ttu-id="8953b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8953b-146">DateTimeOffset</span></span>|<span data-ttu-id="8953b-147">Hora UTC quando o primeiro usuário ingressou na chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-147">UTC time when the first user joined the call.</span></span> <span data-ttu-id="8953b-148">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8953b-148">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8953b-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8953b-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8953b-150">type</span><span class="sxs-lookup"><span data-stu-id="8953b-150">type</span></span>|<span data-ttu-id="8953b-151">string</span><span class="sxs-lookup"><span data-stu-id="8953b-151">string</span></span>|<span data-ttu-id="8953b-152">Indica o tipo da chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-152">Indicates the type of the call.</span></span> <span data-ttu-id="8953b-153">Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8953b-153">Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8953b-154">versão</span><span class="sxs-lookup"><span data-stu-id="8953b-154">version</span></span>|<span data-ttu-id="8953b-155">Int64</span><span class="sxs-lookup"><span data-stu-id="8953b-155">Int64</span></span>|<span data-ttu-id="8953b-156">Versão de aumento monotônico do registro de chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-156">Monotonically increasing version of the call record.</span></span> <span data-ttu-id="8953b-157">Registros de chamada de versão superior com a mesma ID incluem dados adicionais comparados à versão inferior.</span><span class="sxs-lookup"><span data-stu-id="8953b-157">Higher version call records with the same id includes additional data compared to the lower version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8953b-158">Relações</span><span class="sxs-lookup"><span data-stu-id="8953b-158">Relationships</span></span>

| <span data-ttu-id="8953b-159">Relação</span><span class="sxs-lookup"><span data-stu-id="8953b-159">Relationship</span></span> | <span data-ttu-id="8953b-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="8953b-160">Type</span></span>        | <span data-ttu-id="8953b-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="8953b-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8953b-162">sessões</span><span class="sxs-lookup"><span data-stu-id="8953b-162">sessions</span></span>|<span data-ttu-id="8953b-163">coleção [Microsoft. Graph. callRecords. Session](callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="8953b-163">[microsoft.graph.callRecords.session](callrecords-session.md) collection</span></span>|<span data-ttu-id="8953b-164">Lista de sessões envolvidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="8953b-164">List of sessions involved in the call.</span></span> <span data-ttu-id="8953b-165">As chamadas ponto a ponto normalmente têm apenas uma sessão, enquanto as chamadas de grupo normalmente têm pelo menos uma sessão por participante.</span><span class="sxs-lookup"><span data-stu-id="8953b-165">Peer-to-peer calls typically only have one session, whereas group calls typically have at least one session per participant.</span></span> <span data-ttu-id="8953b-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8953b-166">Read-only.</span></span> <span data-ttu-id="8953b-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8953b-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8953b-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8953b-168">JSON representation</span></span>

<span data-ttu-id="8953b-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8953b-169">The following is a JSON representation of the resource.</span></span>

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