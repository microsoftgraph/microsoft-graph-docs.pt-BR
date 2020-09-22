---
title: tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de mudança para obter timeOff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6afbc9537bd56462253944d8df9542e46edbc6bd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090778"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="8cf96-103">tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="8cf96-103">timeOffRequest resource type</span></span>

<span data-ttu-id="8cf96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cf96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cf96-105">Representa um tipo de solicitação de mudança para obter [timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="8cf96-105">Represents a type of shift request to take [timeOff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8cf96-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8cf96-106">Methods</span></span>

| <span data-ttu-id="8cf96-107">Método</span><span class="sxs-lookup"><span data-stu-id="8cf96-107">Method</span></span>       | <span data-ttu-id="8cf96-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8cf96-108">Return Type</span></span> | <span data-ttu-id="8cf96-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cf96-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8cf96-110">Get</span><span class="sxs-lookup"><span data-stu-id="8cf96-110">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="8cf96-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="8cf96-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="8cf96-112">Leia as propriedades e os relacionamentos de um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="8cf96-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="8cf96-113">List</span><span class="sxs-lookup"><span data-stu-id="8cf96-113">List</span></span>](../api/timeoffrequest-list.md) | <span data-ttu-id="8cf96-114">coleção [timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8cf96-114">[timeOffRequest](timeoffrequest.md) collection</span></span> | <span data-ttu-id="8cf96-115">Obtenha a lista de objetos **timeOffRequest** neste cronograma.</span><span class="sxs-lookup"><span data-stu-id="8cf96-115">Get the list of **timeOffRequest** objects in this schedule.</span></span>|
| [<span data-ttu-id="8cf96-116">Delete</span><span class="sxs-lookup"><span data-stu-id="8cf96-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="8cf96-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cf96-117">None</span></span> | <span data-ttu-id="8cf96-118">Excluir um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="8cf96-118">Delete a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="8cf96-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="8cf96-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="8cf96-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cf96-120">None</span></span>|<span data-ttu-id="8cf96-121">Aprovar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="8cf96-121">Approve a time off request.</span></span>|
| [<span data-ttu-id="8cf96-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="8cf96-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="8cf96-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cf96-123">None</span></span>|<span data-ttu-id="8cf96-124">Recusar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="8cf96-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cf96-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cf96-125">Properties</span></span>

| <span data-ttu-id="8cf96-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cf96-126">Property</span></span>     | <span data-ttu-id="8cf96-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cf96-127">Type</span></span>        | <span data-ttu-id="8cf96-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cf96-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cf96-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8cf96-129">endDateTime</span></span>|<span data-ttu-id="8cf96-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cf96-130">DateTimeOffset</span></span>|<span data-ttu-id="8cf96-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8cf96-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8cf96-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8cf96-133">startDateTime</span></span>|<span data-ttu-id="8cf96-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cf96-134">DateTimeOffset</span></span>|<span data-ttu-id="8cf96-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8cf96-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8cf96-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="8cf96-137">timeOffReasonId</span></span>|<span data-ttu-id="8cf96-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cf96-138">String</span></span>|<span data-ttu-id="8cf96-139">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="8cf96-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cf96-140">Relações</span><span class="sxs-lookup"><span data-stu-id="8cf96-140">Relationships</span></span>

<span data-ttu-id="8cf96-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cf96-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cf96-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cf96-142">JSON representation</span></span>

<span data-ttu-id="8cf96-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cf96-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

