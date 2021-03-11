---
title: Tipo de recurso timeOffReason
description: Um motivo válido para fazer o tempo de folga na agenda.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b449f2cb4dcfcd73208d58f8e1e969b9a701e54b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720183"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="b3b97-103">Tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b3b97-103">timeOffReason resource type</span></span>

<span data-ttu-id="b3b97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3b97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b97-105">Um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="b3b97-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b3b97-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3b97-106">Methods</span></span>

| <span data-ttu-id="b3b97-107">Método</span><span class="sxs-lookup"><span data-stu-id="b3b97-107">Method</span></span>       | <span data-ttu-id="b3b97-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3b97-108">Return Type</span></span>  |<span data-ttu-id="b3b97-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b97-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3b97-110">Criar</span><span class="sxs-lookup"><span data-stu-id="b3b97-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="b3b97-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b3b97-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b3b97-112">Crie um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="b3b97-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="b3b97-113">List</span><span class="sxs-lookup"><span data-stu-id="b3b97-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="b3b97-114">[Coleção timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="b3b97-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="b3b97-115">Obter a lista **de timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="b3b97-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="b3b97-116">Get</span><span class="sxs-lookup"><span data-stu-id="b3b97-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="b3b97-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b3b97-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b3b97-118">Obter um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="b3b97-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="b3b97-119">Replace</span><span class="sxs-lookup"><span data-stu-id="b3b97-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="b3b97-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b3b97-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="b3b97-121">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="b3b97-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="b3b97-122">Delete</span><span class="sxs-lookup"><span data-stu-id="b3b97-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="b3b97-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="b3b97-123">None</span></span> | <span data-ttu-id="b3b97-124">Marque um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="b3b97-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3b97-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3b97-125">Properties</span></span>
|<span data-ttu-id="b3b97-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b3b97-126">Name</span></span>          |<span data-ttu-id="b3b97-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3b97-127">Type</span></span>           |<span data-ttu-id="b3b97-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b97-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="b3b97-129">id</span><span class="sxs-lookup"><span data-stu-id="b3b97-129">id</span></span>            |`string`      |<span data-ttu-id="b3b97-130">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="b3b97-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="b3b97-131">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="b3b97-131">displayName</span></span>               | `string`                  | <span data-ttu-id="b3b97-132">O nome do `timeOffReason` .</span><span class="sxs-lookup"><span data-stu-id="b3b97-132">The name of the `timeOffReason`.</span></span> <span data-ttu-id="b3b97-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3b97-133">Required.</span></span> |
| <span data-ttu-id="b3b97-134">iconType</span><span class="sxs-lookup"><span data-stu-id="b3b97-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="b3b97-135">Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span><span class="sxs-lookup"><span data-stu-id="b3b97-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="b3b97-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3b97-136">Required.</span></span> |
| <span data-ttu-id="b3b97-137">isActive</span><span class="sxs-lookup"><span data-stu-id="b3b97-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="b3b97-138">Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="b3b97-138">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="b3b97-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3b97-139">Required.</span></span> |
| <span data-ttu-id="b3b97-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3b97-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b3b97-141">O carimbo de data/hora no `timeOffReason` qual isso foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="b3b97-141">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="b3b97-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3b97-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3b97-143">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b3b97-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="b3b97-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3b97-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="b3b97-145">O carimbo de data/hora no qual `timeOffReason` foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b3b97-145">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="b3b97-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3b97-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3b97-147">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b3b97-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="b3b97-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b3b97-148">lastModifiedBy</span></span>        | [<span data-ttu-id="b3b97-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="b3b97-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="b3b97-150">A identidade da última atualização `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="b3b97-150">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3b97-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3b97-151">JSON representation</span></span>

<span data-ttu-id="b3b97-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3b97-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


