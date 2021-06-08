---
title: Tipo de recurso timeOffReason
description: Um motivo válido para fazer o tempo de folga na agenda.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b236fa6bd55e0af294955286e1443310196688a8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784973"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="8b31f-103">Tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="8b31f-103">timeOffReason resource type</span></span>

<span data-ttu-id="8b31f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b31f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b31f-105">Um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8b31f-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8b31f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b31f-106">Methods</span></span>

| <span data-ttu-id="8b31f-107">Método</span><span class="sxs-lookup"><span data-stu-id="8b31f-107">Method</span></span>       | <span data-ttu-id="8b31f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b31f-108">Return type</span></span>  |<span data-ttu-id="8b31f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b31f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b31f-110">Criar</span><span class="sxs-lookup"><span data-stu-id="8b31f-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="8b31f-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="8b31f-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="8b31f-112">Crie um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="8b31f-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="8b31f-113">List</span><span class="sxs-lookup"><span data-stu-id="8b31f-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="8b31f-114">[Coleção timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="8b31f-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="8b31f-115">Obter a lista **de timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="8b31f-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="8b31f-116">Get</span><span class="sxs-lookup"><span data-stu-id="8b31f-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="8b31f-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="8b31f-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="8b31f-118">Obter um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="8b31f-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="8b31f-119">Replace</span><span class="sxs-lookup"><span data-stu-id="8b31f-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="8b31f-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="8b31f-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="8b31f-121">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="8b31f-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="8b31f-122">Delete</span><span class="sxs-lookup"><span data-stu-id="8b31f-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="8b31f-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8b31f-123">None</span></span> | <span data-ttu-id="8b31f-124">Marque um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="8b31f-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b31f-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b31f-125">Properties</span></span>
|<span data-ttu-id="8b31f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8b31f-126">Name</span></span>          |<span data-ttu-id="8b31f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b31f-127">Type</span></span>           |<span data-ttu-id="8b31f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b31f-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="8b31f-129">id</span><span class="sxs-lookup"><span data-stu-id="8b31f-129">id</span></span>            |`string`      |<span data-ttu-id="8b31f-130">ID do **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="8b31f-130">ID of the **timeOffReason**.</span></span>|
| <span data-ttu-id="8b31f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="8b31f-131">displayName</span></span>               | `string`                  | <span data-ttu-id="8b31f-132">O nome do **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="8b31f-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="8b31f-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b31f-133">Required.</span></span> |
| <span data-ttu-id="8b31f-134">iconType</span><span class="sxs-lookup"><span data-stu-id="8b31f-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="8b31f-135">Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span><span class="sxs-lookup"><span data-stu-id="8b31f-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="8b31f-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b31f-136">Required.</span></span> |
| <span data-ttu-id="8b31f-137">isActive</span><span class="sxs-lookup"><span data-stu-id="8b31f-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="8b31f-138">Indica se o **timeOffReason** pode ser usado ao criar novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="8b31f-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="8b31f-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b31f-139">Required.</span></span> |
| <span data-ttu-id="8b31f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b31f-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8b31f-141">O carimbo de data/hora no **qualOffReason** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="8b31f-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="8b31f-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8b31f-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8b31f-143">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8b31f-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8b31f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b31f-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="8b31f-145">O carimbo de data/hora no **qualOffReason** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8b31f-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="8b31f-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8b31f-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8b31f-147">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8b31f-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8b31f-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8b31f-148">lastModifiedBy</span></span>        | [<span data-ttu-id="8b31f-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="8b31f-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="8b31f-150">A identidade que foi atualizada pela última **vez desta vezOffReason**.</span><span class="sxs-lookup"><span data-stu-id="8b31f-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b31f-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b31f-151">JSON representation</span></span>

<span data-ttu-id="8b31f-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b31f-152">Here is a JSON representation of the resource.</span></span>

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


