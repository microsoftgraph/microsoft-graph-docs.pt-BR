---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8c7d792b834125bdfb8a109c85b2c1f45b18230b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007652"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="24e2d-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24e2d-104">Uma unidade de não trabalho no cronograma.</span><span class="sxs-lookup"><span data-stu-id="24e2d-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="24e2d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="24e2d-105">Methods</span></span>

| <span data-ttu-id="24e2d-106">Método</span><span class="sxs-lookup"><span data-stu-id="24e2d-106">Method</span></span>       | <span data-ttu-id="24e2d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="24e2d-107">Return Type</span></span>  |<span data-ttu-id="24e2d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e2d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24e2d-109">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="24e2d-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-110">timeOff</span></span>](timeoff.md) | <span data-ttu-id="24e2d-111">Criar um novo `timeOff` objeto.</span><span class="sxs-lookup"><span data-stu-id="24e2d-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="24e2d-112">Listar timeoffss</span><span class="sxs-lookup"><span data-stu-id="24e2d-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="24e2d-113">coleção [timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="24e2d-113">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="24e2d-114">Obtenha a lista de `timeOff` objetos nesse cronograma.</span><span class="sxs-lookup"><span data-stu-id="24e2d-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="24e2d-115">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="24e2d-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-116">timeOff</span></span>](timeoff.md) | <span data-ttu-id="24e2d-117">Obter um `timeOff` por ID.</span><span class="sxs-lookup"><span data-stu-id="24e2d-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="24e2d-118">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="24e2d-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-119">timeOff</span></span>](timeoff.md) | <span data-ttu-id="24e2d-120">Substituir um `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="24e2d-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="24e2d-121">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="24e2d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24e2d-122">None</span></span> | <span data-ttu-id="24e2d-123">Excluir uma `timeOff` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="24e2d-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="24e2d-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24e2d-124">Properties</span></span>
|<span data-ttu-id="24e2d-125">Nome</span><span class="sxs-lookup"><span data-stu-id="24e2d-125">Name</span></span>          |<span data-ttu-id="24e2d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="24e2d-126">Type</span></span>           |<span data-ttu-id="24e2d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e2d-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="24e2d-128">id</span><span class="sxs-lookup"><span data-stu-id="24e2d-128">id</span></span>            |`string`      |<span data-ttu-id="24e2d-129">A ID da tarefa `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="24e2d-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="24e2d-130">userId</span><span class="sxs-lookup"><span data-stu-id="24e2d-130">userId</span></span>            |`string`      |<span data-ttu-id="24e2d-131">ID do usuário atribuído ao `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="24e2d-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="24e2d-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e2d-132">Required.</span></span>|
| <span data-ttu-id="24e2d-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-133">sharedTimeOff</span></span>     | [<span data-ttu-id="24e2d-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="24e2d-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="24e2d-135">A versão compartilhada desse `timeOff` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="24e2d-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="24e2d-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e2d-136">Required.</span></span>|
| <span data-ttu-id="24e2d-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="24e2d-137">draftTimeOff</span></span>      | [<span data-ttu-id="24e2d-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="24e2d-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="24e2d-139">A versão de rascunho desse `timeOff` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="24e2d-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="24e2d-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e2d-140">Required.</span></span>|
| <span data-ttu-id="24e2d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24e2d-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="24e2d-142">O carimbo de data/hora `timeOff` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="24e2d-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="24e2d-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24e2d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24e2d-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="24e2d-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="24e2d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24e2d-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="24e2d-146">O carimbo de data/hora `timeOff` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="24e2d-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="24e2d-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24e2d-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24e2d-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="24e2d-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="24e2d-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="24e2d-149">lastModifiedBy</span></span>        | [<span data-ttu-id="24e2d-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="24e2d-150">identitySet</span></span>](identityset.md)        |<span data-ttu-id="24e2d-151">A identidade da última atualização `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="24e2d-151">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24e2d-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24e2d-152">JSON representation</span></span>

<span data-ttu-id="24e2d-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24e2d-153">Here is a JSON representation of the resource.</span></span>

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
