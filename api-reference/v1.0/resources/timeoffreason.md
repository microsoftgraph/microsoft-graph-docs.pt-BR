---
title: Tipo de recurso timeOffReason
description: Representa um motivo válido para o tempo de folga na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9d73892d8bcd8ca6beba8be66fe0acc1f036e41e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720085"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="04452-103">Tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04452-103">timeOffReason resource type</span></span>

<span data-ttu-id="04452-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04452-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04452-105">Representa um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="04452-105">Represents a valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="04452-106">Methods</span><span class="sxs-lookup"><span data-stu-id="04452-106">Methods</span></span>

| <span data-ttu-id="04452-107">Método</span><span class="sxs-lookup"><span data-stu-id="04452-107">Method</span></span>       | <span data-ttu-id="04452-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04452-108">Return Type</span></span>  |<span data-ttu-id="04452-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="04452-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04452-110">List</span><span class="sxs-lookup"><span data-stu-id="04452-110">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="04452-111">[Coleção timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="04452-111">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="04452-112">Obter a lista **de timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="04452-112">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="04452-113">Create</span><span class="sxs-lookup"><span data-stu-id="04452-113">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="04452-114">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04452-114">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04452-115">Crie um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="04452-115">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="04452-116">Get</span><span class="sxs-lookup"><span data-stu-id="04452-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="04452-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04452-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04452-118">Obter um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="04452-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="04452-119">Replace</span><span class="sxs-lookup"><span data-stu-id="04452-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="04452-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04452-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04452-121">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="04452-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="04452-122">Delete</span><span class="sxs-lookup"><span data-stu-id="04452-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="04452-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04452-123">None</span></span> | <span data-ttu-id="04452-124">Marque um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="04452-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="04452-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04452-125">Properties</span></span>
|<span data-ttu-id="04452-126">Nome</span><span class="sxs-lookup"><span data-stu-id="04452-126">Name</span></span>          |<span data-ttu-id="04452-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="04452-127">Type</span></span>           |<span data-ttu-id="04452-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="04452-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="04452-129">id</span><span class="sxs-lookup"><span data-stu-id="04452-129">id</span></span>            |`string`      |<span data-ttu-id="04452-130">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="04452-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="04452-131">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="04452-131">displayName</span></span>               | `string`                  | <span data-ttu-id="04452-132">O nome do **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="04452-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="04452-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04452-133">Required.</span></span> |
| <span data-ttu-id="04452-134">iconType</span><span class="sxs-lookup"><span data-stu-id="04452-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="04452-135">Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span><span class="sxs-lookup"><span data-stu-id="04452-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="04452-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04452-136">Required.</span></span> |
| <span data-ttu-id="04452-137">isActive</span><span class="sxs-lookup"><span data-stu-id="04452-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="04452-138">Indica se o **timeOffReason** pode ser usado ao criar novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="04452-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="04452-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04452-139">Required.</span></span> |
| <span data-ttu-id="04452-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04452-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="04452-141">O carimbo de data/hora no **qualOffReason** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="04452-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="04452-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="04452-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04452-143">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="04452-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="04452-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04452-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="04452-145">O carimbo de data/hora no **qualOffReason** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="04452-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="04452-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="04452-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04452-147">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="04452-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="04452-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="04452-148">lastModifiedBy</span></span>        | [<span data-ttu-id="04452-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="04452-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="04452-150">A identidade que foi atualizada pela última **vez desta vezOffReason**.</span><span class="sxs-lookup"><span data-stu-id="04452-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04452-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04452-151">JSON representation</span></span>

<span data-ttu-id="04452-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04452-152">The following is a JSON representation of the resource.</span></span>

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

