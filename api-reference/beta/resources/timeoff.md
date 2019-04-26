---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 848365a812053b7788db37395bee8662d69cda37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342009"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="b0f97-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0f97-104">Uma unidade de não trabalho no cronograma.</span><span class="sxs-lookup"><span data-stu-id="b0f97-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="b0f97-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0f97-105">Methods</span></span>

| <span data-ttu-id="b0f97-106">Método</span><span class="sxs-lookup"><span data-stu-id="b0f97-106">Method</span></span>       | <span data-ttu-id="b0f97-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0f97-107">Return Type</span></span>  |<span data-ttu-id="b0f97-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0f97-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0f97-109">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="b0f97-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b0f97-111">Criar um novo `timeOff` objeto.</span><span class="sxs-lookup"><span data-stu-id="b0f97-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="b0f97-112">Listar timeOffss</span><span class="sxs-lookup"><span data-stu-id="b0f97-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="b0f97-113">coleção [timeOff](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="b0f97-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="b0f97-114">Obtenha a lista de `timeOff` objetos nesse cronograma.</span><span class="sxs-lookup"><span data-stu-id="b0f97-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="b0f97-115">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="b0f97-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b0f97-117">Obter um `timeOff` por ID.</span><span class="sxs-lookup"><span data-stu-id="b0f97-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="b0f97-118">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="b0f97-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b0f97-120">Substituir um `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b0f97-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="b0f97-121">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="b0f97-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0f97-122">None</span></span> | <span data-ttu-id="b0f97-123">Excluir uma `timeOff` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="b0f97-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0f97-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0f97-124">Properties</span></span>
|<span data-ttu-id="b0f97-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b0f97-125">Name</span></span>          |<span data-ttu-id="b0f97-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0f97-126">Type</span></span>           |<span data-ttu-id="b0f97-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0f97-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b0f97-128">id</span><span class="sxs-lookup"><span data-stu-id="b0f97-128">id</span></span>            |`string`      |<span data-ttu-id="b0f97-129">A ID da tarefa `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b0f97-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="b0f97-130">userId</span><span class="sxs-lookup"><span data-stu-id="b0f97-130">userId</span></span>            |`string`      |<span data-ttu-id="b0f97-131">ID do usuário atribuído ao `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b0f97-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="b0f97-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0f97-132">Required.</span></span>|
| <span data-ttu-id="b0f97-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-133">sharedTimeOff</span></span>     | [<span data-ttu-id="b0f97-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b0f97-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="b0f97-135">A versão compartilhada desse `timeOff` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="b0f97-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="b0f97-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0f97-136">Required.</span></span>|
| <span data-ttu-id="b0f97-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="b0f97-137">draftTimeOff</span></span>      | [<span data-ttu-id="b0f97-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b0f97-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="b0f97-139">A versão de rascunho desse `timeOff` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="b0f97-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="b0f97-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0f97-140">Required.</span></span>|
| <span data-ttu-id="b0f97-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f97-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b0f97-142">O carimbo de data/hora `timeOff` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="b0f97-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="b0f97-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b0f97-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0f97-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b0f97-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b0f97-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f97-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="b0f97-146">O carimbo de data/hora `timeOff` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0f97-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="b0f97-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b0f97-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0f97-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b0f97-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b0f97-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b0f97-149">lastModifiedBy</span></span>        | [<span data-ttu-id="b0f97-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="b0f97-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="b0f97-151">A identidade da última atualização `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b0f97-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0f97-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0f97-152">JSON representation</span></span>

<span data-ttu-id="b0f97-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0f97-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
