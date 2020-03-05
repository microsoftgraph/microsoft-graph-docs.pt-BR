---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 3ff9edf6bf3834faf5d91773b6c94ecbc4158d79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519733"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="b9243-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-103">timeOff resource type</span></span>

<span data-ttu-id="b9243-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9243-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9243-105">Uma unidade de não funcionar em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="b9243-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="b9243-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b9243-106">Methods</span></span>

| <span data-ttu-id="b9243-107">Método</span><span class="sxs-lookup"><span data-stu-id="b9243-107">Method</span></span>       | <span data-ttu-id="b9243-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b9243-108">Return Type</span></span>  |<span data-ttu-id="b9243-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9243-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9243-110">Criar</span><span class="sxs-lookup"><span data-stu-id="b9243-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="b9243-111">timeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="b9243-112">Criar um novo objeto **timeOff** .</span><span class="sxs-lookup"><span data-stu-id="b9243-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="b9243-113">List</span><span class="sxs-lookup"><span data-stu-id="b9243-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="b9243-114">coleção [timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="b9243-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="b9243-115">Obtenha a lista de objetos **timeOff** neste cronograma.</span><span class="sxs-lookup"><span data-stu-id="b9243-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|<span data-ttu-id="b9243-116">[Get (.. /api/timeoff-get.md)</span><span class="sxs-lookup"><span data-stu-id="b9243-116">[Get (../api/timeoff-get.md)</span></span> | [<span data-ttu-id="b9243-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="b9243-118">Obtenha um objeto **timeOff** por ID.</span><span class="sxs-lookup"><span data-stu-id="b9243-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="b9243-119">Replace</span><span class="sxs-lookup"><span data-stu-id="b9243-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="b9243-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="b9243-121">Substituir um objeto **timeOff** .</span><span class="sxs-lookup"><span data-stu-id="b9243-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="b9243-122">Delete</span><span class="sxs-lookup"><span data-stu-id="b9243-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="b9243-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9243-123">None</span></span> | <span data-ttu-id="b9243-124">Excluir um objeto **timeOff** da agenda.</span><span class="sxs-lookup"><span data-stu-id="b9243-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9243-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9243-125">Properties</span></span>
|<span data-ttu-id="b9243-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b9243-126">Name</span></span>          |<span data-ttu-id="b9243-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9243-127">Type</span></span>           |<span data-ttu-id="b9243-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9243-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b9243-129">id</span><span class="sxs-lookup"><span data-stu-id="b9243-129">id</span></span>            |`string`      |<span data-ttu-id="b9243-130">A ID da tarefa `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b9243-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="b9243-131">userId</span><span class="sxs-lookup"><span data-stu-id="b9243-131">userId</span></span>            |`string`      |<span data-ttu-id="b9243-132">ID do usuário atribuído ao `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b9243-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="b9243-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9243-133">Required.</span></span>|
| <span data-ttu-id="b9243-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-134">sharedTimeOff</span></span>     | [<span data-ttu-id="b9243-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b9243-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="b9243-136">A versão compartilhada desse `timeOff` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="b9243-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="b9243-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9243-137">Required.</span></span>|
| <span data-ttu-id="b9243-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="b9243-138">draftTimeOff</span></span>      | [<span data-ttu-id="b9243-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b9243-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="b9243-140">A versão de rascunho desse `timeOff` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="b9243-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="b9243-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9243-141">Required.</span></span>|
| <span data-ttu-id="b9243-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9243-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b9243-143">O carimbo de data/hora `timeOff` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="b9243-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="b9243-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b9243-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9243-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b9243-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b9243-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9243-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="b9243-147">O carimbo de data/hora `timeOff` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b9243-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="b9243-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b9243-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9243-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b9243-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b9243-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b9243-150">lastModifiedBy</span></span>        | [<span data-ttu-id="b9243-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9243-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="b9243-152">A identidade da última atualização `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b9243-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9243-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9243-153">JSON representation</span></span>

<span data-ttu-id="b9243-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9243-154">Here is a JSON representation of the resource.</span></span>

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
