---
title: tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de mudança para obter timeoff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73fa72d403bd20e6a966b01a0529d09689e5ed66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519712"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="caa0a-103">tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="caa0a-103">timeOffRequest resource type</span></span>

<span data-ttu-id="caa0a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="caa0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caa0a-105">Representa um tipo de solicitação de mudança para obter [timeoff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="caa0a-105">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="caa0a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="caa0a-106">Methods</span></span>

| <span data-ttu-id="caa0a-107">Método</span><span class="sxs-lookup"><span data-stu-id="caa0a-107">Method</span></span>       | <span data-ttu-id="caa0a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="caa0a-108">Return Type</span></span> | <span data-ttu-id="caa0a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="caa0a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="caa0a-110">Get</span><span class="sxs-lookup"><span data-stu-id="caa0a-110">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="caa0a-111">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="caa0a-111">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="caa0a-112">Leia as propriedades e os relacionamentos de um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="caa0a-112">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="caa0a-113">Update</span><span class="sxs-lookup"><span data-stu-id="caa0a-113">Update</span></span>](../api/timeoffrequest-update.md) | [<span data-ttu-id="caa0a-114">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="caa0a-114">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="caa0a-115">Atualizar um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="caa0a-115">Update a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="caa0a-116">Delete</span><span class="sxs-lookup"><span data-stu-id="caa0a-116">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="caa0a-117">None</span><span class="sxs-lookup"><span data-stu-id="caa0a-117">None</span></span> | <span data-ttu-id="caa0a-118">Excluir um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="caa0a-118">Delete a **timeOffRequest** object.</span></span> |
|[<span data-ttu-id="caa0a-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="caa0a-119">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="caa0a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caa0a-120">None</span></span>|<span data-ttu-id="caa0a-121">Aprovar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="caa0a-121">Approve a time off request.</span></span>|
|[<span data-ttu-id="caa0a-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="caa0a-122">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="caa0a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caa0a-123">None</span></span>|<span data-ttu-id="caa0a-124">Recusar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="caa0a-124">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="caa0a-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="caa0a-125">Properties</span></span>

| <span data-ttu-id="caa0a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caa0a-126">Property</span></span>     | <span data-ttu-id="caa0a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="caa0a-127">Type</span></span>        | <span data-ttu-id="caa0a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="caa0a-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="caa0a-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="caa0a-129">endDateTime</span></span>|<span data-ttu-id="caa0a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa0a-130">DateTimeOffset</span></span>|<span data-ttu-id="caa0a-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="caa0a-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="caa0a-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="caa0a-133">startDateTime</span></span>|<span data-ttu-id="caa0a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa0a-134">DateTimeOffset</span></span>|<span data-ttu-id="caa0a-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="caa0a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="caa0a-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="caa0a-137">timeOffReasonId</span></span>|<span data-ttu-id="caa0a-138">String</span><span class="sxs-lookup"><span data-stu-id="caa0a-138">String</span></span>|<span data-ttu-id="caa0a-139">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="caa0a-139">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caa0a-140">Relações</span><span class="sxs-lookup"><span data-stu-id="caa0a-140">Relationships</span></span>

<span data-ttu-id="caa0a-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caa0a-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="caa0a-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="caa0a-142">JSON representation</span></span>

<span data-ttu-id="caa0a-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="caa0a-143">The following is a JSON representation of the resource.</span></span>

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
