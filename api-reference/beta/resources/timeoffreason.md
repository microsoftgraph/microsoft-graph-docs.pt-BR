---
title: tipo de recurso timeOffReason
description: Uma razão válida para ser demorada no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 514ca74bb9826546e95f225e394e8fc07a0f674f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866515"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="6c2d1-103">tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6c2d1-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c2d1-104">Uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="6c2d1-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6c2d1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c2d1-105">Methods</span></span>

| <span data-ttu-id="6c2d1-106">Método</span><span class="sxs-lookup"><span data-stu-id="6c2d1-106">Method</span></span>       | <span data-ttu-id="6c2d1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c2d1-107">Return Type</span></span>  |<span data-ttu-id="6c2d1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c2d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c2d1-109">Criar</span><span class="sxs-lookup"><span data-stu-id="6c2d1-109">Create</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="6c2d1-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6c2d1-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="6c2d1-111">Criar um novo **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-111">Create a new **timeOffReason**.</span></span>|
|[<span data-ttu-id="6c2d1-112">List</span><span class="sxs-lookup"><span data-stu-id="6c2d1-112">List</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="6c2d1-113">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="6c2d1-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="6c2d1-114">Obtenha a lista de **timeOffReason** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-114">Get the list of **timeOffReason** in a schedule.</span></span>|
|[<span data-ttu-id="6c2d1-115">Get</span><span class="sxs-lookup"><span data-stu-id="6c2d1-115">Get</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="6c2d1-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6c2d1-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="6c2d1-117">Obtenha um **timeOffReason** por ID.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-117">Get a **timeOffReason** by ID.</span></span>|
|[<span data-ttu-id="6c2d1-118">Replace</span><span class="sxs-lookup"><span data-stu-id="6c2d1-118">Replace</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="6c2d1-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6c2d1-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="6c2d1-120">Substitua um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-120">Replace a **timeOffReason**.</span></span>|
|[<span data-ttu-id="6c2d1-121">Delete</span><span class="sxs-lookup"><span data-stu-id="6c2d1-121">Delete</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="6c2d1-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c2d1-122">None</span></span> | <span data-ttu-id="6c2d1-123">Marcar um **timeOffReason** como inativo.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-123">Mark a **timeOffReason** as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c2d1-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c2d1-124">Properties</span></span>
|<span data-ttu-id="6c2d1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6c2d1-125">Name</span></span>          |<span data-ttu-id="6c2d1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c2d1-126">Type</span></span>           |<span data-ttu-id="6c2d1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c2d1-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="6c2d1-128">id</span><span class="sxs-lookup"><span data-stu-id="6c2d1-128">id</span></span>            |`string`      |<span data-ttu-id="6c2d1-129">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="6c2d1-130">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="6c2d1-130">displayName</span></span>               | `string`                  | <span data-ttu-id="6c2d1-131">O nome do `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="6c2d1-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-132">Required.</span></span> |
| <span data-ttu-id="6c2d1-133">icontype</span><span class="sxs-lookup"><span data-stu-id="6c2d1-133">iconType</span></span> | `timeOffReasonIconType`   | <span data-ttu-id="6c2d1-134">Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="6c2d1-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-135">Required.</span></span> |
| <span data-ttu-id="6c2d1-136">isActive</span><span class="sxs-lookup"><span data-stu-id="6c2d1-136">isActive</span></span>          |`Boolean`      | <span data-ttu-id="6c2d1-137">Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="6c2d1-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-138">Required.</span></span> |
| <span data-ttu-id="6c2d1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c2d1-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="6c2d1-140">O carimbo de data/hora `timeOffReason` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="6c2d1-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c2d1-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6c2d1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c2d1-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="6c2d1-144">O carimbo de data/hora `timeOffReason` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="6c2d1-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c2d1-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6c2d1-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c2d1-147">lastModifiedBy</span></span>        | [<span data-ttu-id="6c2d1-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c2d1-148">identitySet</span></span>](identityset.md)        |<span data-ttu-id="6c2d1-149">A identidade da última atualização `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-149">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c2d1-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c2d1-150">JSON representation</span></span>

<span data-ttu-id="6c2d1-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c2d1-151">Here is a JSON representation of the resource.</span></span>

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
