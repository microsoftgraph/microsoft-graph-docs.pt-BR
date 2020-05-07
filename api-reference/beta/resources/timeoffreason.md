---
title: tipo de recurso timeOffReason
description: Uma razão válida para ser demorada no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c766a29a75bfe96ca6d0175b3017f4a310448c2d
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154441"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="9cc6f-103">tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="9cc6f-103">timeOffReason resource type</span></span>

<span data-ttu-id="9cc6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc6f-105">Uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="9cc6f-105">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9cc6f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9cc6f-106">Methods</span></span>

| <span data-ttu-id="9cc6f-107">Método</span><span class="sxs-lookup"><span data-stu-id="9cc6f-107">Method</span></span>       | <span data-ttu-id="9cc6f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9cc6f-108">Return Type</span></span>  |<span data-ttu-id="9cc6f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc6f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cc6f-110">Criar</span><span class="sxs-lookup"><span data-stu-id="9cc6f-110">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="9cc6f-111">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="9cc6f-111">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="9cc6f-112">Criar um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-112">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="9cc6f-113">List</span><span class="sxs-lookup"><span data-stu-id="9cc6f-113">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="9cc6f-114">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="9cc6f-114">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="9cc6f-115">Obtenha a lista de **timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-115">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="9cc6f-116">Get</span><span class="sxs-lookup"><span data-stu-id="9cc6f-116">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="9cc6f-117">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="9cc6f-117">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="9cc6f-118">Obtenha um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-118">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="9cc6f-119">Replace</span><span class="sxs-lookup"><span data-stu-id="9cc6f-119">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="9cc6f-120">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="9cc6f-120">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="9cc6f-121">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-121">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="9cc6f-122">Delete</span><span class="sxs-lookup"><span data-stu-id="9cc6f-122">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="9cc6f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9cc6f-123">None</span></span> | <span data-ttu-id="9cc6f-124">Marcar um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-124">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cc6f-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cc6f-125">Properties</span></span>
|<span data-ttu-id="9cc6f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9cc6f-126">Name</span></span>          |<span data-ttu-id="9cc6f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc6f-127">Type</span></span>           |<span data-ttu-id="9cc6f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc6f-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="9cc6f-129">id</span><span class="sxs-lookup"><span data-stu-id="9cc6f-129">id</span></span>            |`string`      |<span data-ttu-id="9cc6f-130">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-130">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="9cc6f-131">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="9cc6f-131">displayName</span></span>               | `string`                  | <span data-ttu-id="9cc6f-132">O nome do `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-132">The name of the `timeOffReason`.</span></span> <span data-ttu-id="9cc6f-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-133">Required.</span></span> |
| <span data-ttu-id="9cc6f-134">icontype</span><span class="sxs-lookup"><span data-stu-id="9cc6f-134">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="9cc6f-135">Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-135">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="9cc6f-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-136">Required.</span></span> |
| <span data-ttu-id="9cc6f-137">isActive</span><span class="sxs-lookup"><span data-stu-id="9cc6f-137">isActive</span></span>          |`Boolean`      | <span data-ttu-id="9cc6f-138">Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-138">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="9cc6f-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-139">Required.</span></span> |
| <span data-ttu-id="9cc6f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cc6f-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="9cc6f-141">O carimbo de data/hora `timeOffReason` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-141">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="9cc6f-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cc6f-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9cc6f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cc6f-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="9cc6f-145">O carimbo de data/hora `timeOffReason` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-145">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="9cc6f-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cc6f-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9cc6f-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9cc6f-148">lastModifiedBy</span></span>        | [<span data-ttu-id="9cc6f-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="9cc6f-149">identitySet</span></span>](identityset.md)        |<span data-ttu-id="9cc6f-150">A identidade da última atualização `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-150">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cc6f-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cc6f-151">JSON representation</span></span>

<span data-ttu-id="9cc6f-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cc6f-152">Here is a JSON representation of the resource.</span></span>

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
