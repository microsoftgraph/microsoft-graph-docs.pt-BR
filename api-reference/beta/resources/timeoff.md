---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657795"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="6e596-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e596-104">Uma unidade de não trabalho no cronograma.</span><span class="sxs-lookup"><span data-stu-id="6e596-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="6e596-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e596-105">Methods</span></span>

| <span data-ttu-id="6e596-106">Método</span><span class="sxs-lookup"><span data-stu-id="6e596-106">Method</span></span>       | <span data-ttu-id="6e596-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e596-107">Return Type</span></span>  |<span data-ttu-id="6e596-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e596-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e596-109">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="6e596-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="6e596-111">Criar um novo `timeOff` objeto.</span><span class="sxs-lookup"><span data-stu-id="6e596-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="6e596-112">Listar timeOffss</span><span class="sxs-lookup"><span data-stu-id="6e596-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="6e596-113">coleção [timeOff](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="6e596-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="6e596-114">Obtenha a lista de `timeOff` objetos nesse cronograma.</span><span class="sxs-lookup"><span data-stu-id="6e596-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="6e596-115">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="6e596-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="6e596-117">Obter a `timeOff` por ID.</span><span class="sxs-lookup"><span data-stu-id="6e596-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="6e596-118">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="6e596-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="6e596-120">Substitua um `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="6e596-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="6e596-121">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="6e596-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e596-122">None</span></span> | <span data-ttu-id="6e596-123">Excluir uma `timeOff` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="6e596-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e596-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e596-124">Properties</span></span>
|<span data-ttu-id="6e596-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6e596-125">Name</span></span>          |<span data-ttu-id="6e596-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e596-126">Type</span></span>           |<span data-ttu-id="6e596-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e596-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6e596-128">id</span><span class="sxs-lookup"><span data-stu-id="6e596-128">id</span></span>            |`string`      |<span data-ttu-id="6e596-129">ID do `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="6e596-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="6e596-130">userId</span><span class="sxs-lookup"><span data-stu-id="6e596-130">userId</span></span>            |`string`      |<span data-ttu-id="6e596-131">ID do usuário atribuído ao `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="6e596-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="6e596-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e596-132">Required.</span></span>|
| <span data-ttu-id="6e596-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-133">sharedTimeOff</span></span>     |`[timeOffItem](timeoffitem.md)`  |<span data-ttu-id="6e596-134">A versão compartilhada desse `timeOff` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="6e596-134">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="6e596-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e596-135">Required.</span></span>|
| <span data-ttu-id="6e596-136">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="6e596-136">draftTimeOff</span></span>      |`[timeOffItem](timeoffitem.md)`        |<span data-ttu-id="6e596-137">A versão de rascunho desse `timeOff` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="6e596-137">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="6e596-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e596-138">Required.</span></span>|
| <span data-ttu-id="6e596-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e596-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="6e596-140">O carimbo de data/hora `timeOff` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="6e596-140">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="6e596-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6e596-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6e596-142">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="6e596-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6e596-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e596-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="6e596-144">O carimbo de data/hora `timeOff` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6e596-144">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="6e596-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6e596-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6e596-146">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="6e596-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6e596-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6e596-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="6e596-148">A identidade que foi atualizada pela `timeOff`última vez.</span><span class="sxs-lookup"><span data-stu-id="6e596-148">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e596-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e596-149">JSON representation</span></span>

<span data-ttu-id="6e596-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e596-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
