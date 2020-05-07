---
title: tipo de recurso timeOffReason
description: Representa uma razão válida para ser demorada no cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: ef852fa92217b32812340fd17b14465a5f4cbba3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154903"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="99174-103">tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="99174-103">timeOffReason resource type</span></span>

<span data-ttu-id="99174-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99174-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99174-105">Representa uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="99174-105">Represents a valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="99174-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="99174-106">Methods</span></span>

| <span data-ttu-id="99174-107">Método</span><span class="sxs-lookup"><span data-stu-id="99174-107">Method</span></span>       | <span data-ttu-id="99174-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99174-108">Return Type</span></span>  |<span data-ttu-id="99174-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99174-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99174-110">List</span><span class="sxs-lookup"><span data-stu-id="99174-110">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="99174-111">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="99174-111">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="99174-112">Obtenha a lista de **timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="99174-112">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="99174-113">Create</span><span class="sxs-lookup"><span data-stu-id="99174-113">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="99174-114">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="99174-114">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="99174-115">Criar um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="99174-115">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="99174-116">Get</span><span class="sxs-lookup"><span data-stu-id="99174-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="99174-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="99174-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="99174-118">Obtenha um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="99174-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="99174-119">Replace</span><span class="sxs-lookup"><span data-stu-id="99174-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="99174-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="99174-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="99174-121">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="99174-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="99174-122">Delete</span><span class="sxs-lookup"><span data-stu-id="99174-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="99174-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99174-123">None</span></span> | <span data-ttu-id="99174-124">Marcar um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="99174-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="99174-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99174-125">Properties</span></span>
|<span data-ttu-id="99174-126">Nome</span><span class="sxs-lookup"><span data-stu-id="99174-126">Name</span></span>          |<span data-ttu-id="99174-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="99174-127">Type</span></span>           |<span data-ttu-id="99174-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="99174-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="99174-129">id</span><span class="sxs-lookup"><span data-stu-id="99174-129">id</span></span>            |`string`      |<span data-ttu-id="99174-130">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="99174-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="99174-131">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="99174-131">displayName</span></span>               | `string`                  | <span data-ttu-id="99174-132">O nome do **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="99174-132">The name of the **timeOffReason**.</span></span> <span data-ttu-id="99174-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99174-133">Required.</span></span> |
| <span data-ttu-id="99174-134">icontype</span><span class="sxs-lookup"><span data-stu-id="99174-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="99174-135">Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado.</span><span class="sxs-lookup"><span data-stu-id="99174-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="99174-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99174-136">Required.</span></span> |
| <span data-ttu-id="99174-137">isActive</span><span class="sxs-lookup"><span data-stu-id="99174-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="99174-138">Indica se o **timeOffReason** pode ser usado ao criar novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="99174-138">Indicates whether the **timeOffReason** can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="99174-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99174-139">Required.</span></span> |
| <span data-ttu-id="99174-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99174-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="99174-141">O carimbo de data/hora em que este **timeOffReason** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="99174-141">The time stamp on which this **timeOffReason** was first created.</span></span> <span data-ttu-id="99174-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="99174-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99174-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="99174-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="99174-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99174-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="99174-145">O carimbo de data/hora em que este **timeOffReason** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="99174-145">The time stamp on which this **timeOffReason** was last updated.</span></span> <span data-ttu-id="99174-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="99174-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99174-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="99174-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="99174-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="99174-148">lastModifiedBy</span></span>        | [<span data-ttu-id="99174-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="99174-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="99174-150">A identidade que atualizou pela última vez este **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="99174-150">The identity that last updated this **timeOffReason**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99174-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99174-151">JSON representation</span></span>

<span data-ttu-id="99174-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99174-152">The following is a JSON representation of the resource.</span></span>

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
