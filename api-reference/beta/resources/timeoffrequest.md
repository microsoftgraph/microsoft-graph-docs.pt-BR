---
title: tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de mudança para obter timeoff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 28be6904b64b89c6386bd25a4ced71f76fdc4088
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895564"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="e68b6-103">tipo de recurso timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="e68b6-103">timeOffRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e68b6-104">Representa um tipo de solicitação de mudança para obter [timeoff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="e68b6-104">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e68b6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e68b6-105">Methods</span></span>

| <span data-ttu-id="e68b6-106">Método</span><span class="sxs-lookup"><span data-stu-id="e68b6-106">Method</span></span>       | <span data-ttu-id="e68b6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e68b6-107">Return Type</span></span> | <span data-ttu-id="e68b6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e68b6-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e68b6-109">Get</span><span class="sxs-lookup"><span data-stu-id="e68b6-109">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="e68b6-110">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="e68b6-110">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="e68b6-111">Leia as propriedades e os relacionamentos de um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="e68b6-111">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="e68b6-112">Update</span><span class="sxs-lookup"><span data-stu-id="e68b6-112">Update</span></span>](../api/timeoffrequest-update.md) | [<span data-ttu-id="e68b6-113">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="e68b6-113">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="e68b6-114">Atualizar um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="e68b6-114">Update a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="e68b6-115">Delete</span><span class="sxs-lookup"><span data-stu-id="e68b6-115">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="e68b6-116">None</span><span class="sxs-lookup"><span data-stu-id="e68b6-116">None</span></span> | <span data-ttu-id="e68b6-117">Excluir um objeto **timeOffRequest** .</span><span class="sxs-lookup"><span data-stu-id="e68b6-117">Delete a **timeOffRequest** object.</span></span> |
|[<span data-ttu-id="e68b6-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="e68b6-118">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="e68b6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e68b6-119">None</span></span>|<span data-ttu-id="e68b6-120">Aprovar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e68b6-120">Approve a time off request.</span></span>|
|[<span data-ttu-id="e68b6-121">Aceito</span><span class="sxs-lookup"><span data-stu-id="e68b6-121">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="e68b6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e68b6-122">None</span></span>|<span data-ttu-id="e68b6-123">Recusar uma solicitação de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e68b6-123">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="e68b6-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e68b6-124">Properties</span></span>

| <span data-ttu-id="e68b6-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e68b6-125">Property</span></span>     | <span data-ttu-id="e68b6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e68b6-126">Type</span></span>        | <span data-ttu-id="e68b6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e68b6-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e68b6-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e68b6-128">endDateTime</span></span>|<span data-ttu-id="e68b6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e68b6-129">DateTimeOffset</span></span>|<span data-ttu-id="e68b6-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e68b6-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e68b6-132">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e68b6-132">startDateTime</span></span>|<span data-ttu-id="e68b6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e68b6-133">DateTimeOffset</span></span>|<span data-ttu-id="e68b6-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e68b6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e68b6-136">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="e68b6-136">timeOffReasonId</span></span>|<span data-ttu-id="e68b6-137">String</span><span class="sxs-lookup"><span data-stu-id="e68b6-137">String</span></span>|<span data-ttu-id="e68b6-138">O motivo da folga.</span><span class="sxs-lookup"><span data-stu-id="e68b6-138">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68b6-139">Relações</span><span class="sxs-lookup"><span data-stu-id="e68b6-139">Relationships</span></span>

<span data-ttu-id="e68b6-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e68b6-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e68b6-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e68b6-141">JSON representation</span></span>

<span data-ttu-id="e68b6-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e68b6-142">The following is a JSON representation of the resource.</span></span>

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
