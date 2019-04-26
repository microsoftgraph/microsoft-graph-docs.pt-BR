---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582840"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="c22ad-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c22ad-104">Uma unidade de não trabalho no cronograma.</span><span class="sxs-lookup"><span data-stu-id="c22ad-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="c22ad-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c22ad-105">Methods</span></span>

| <span data-ttu-id="c22ad-106">Método</span><span class="sxs-lookup"><span data-stu-id="c22ad-106">Method</span></span>       | <span data-ttu-id="c22ad-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c22ad-107">Return Type</span></span>  |<span data-ttu-id="c22ad-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c22ad-109">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="c22ad-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="c22ad-111">Criar um novo `timeOff` objeto.</span><span class="sxs-lookup"><span data-stu-id="c22ad-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="c22ad-112">Listar timeOffss</span><span class="sxs-lookup"><span data-stu-id="c22ad-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="c22ad-113">coleção [timeOff](timeOff.md)</span><span class="sxs-lookup"><span data-stu-id="c22ad-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="c22ad-114">Obtenha a lista de `timeOff` objetos nesse cronograma.</span><span class="sxs-lookup"><span data-stu-id="c22ad-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="c22ad-115">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="c22ad-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="c22ad-117">Obter um `timeOff` por ID.</span><span class="sxs-lookup"><span data-stu-id="c22ad-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="c22ad-118">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="c22ad-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="c22ad-120">Substituir um `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="c22ad-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="c22ad-121">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="c22ad-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c22ad-122">None</span></span> | <span data-ttu-id="c22ad-123">Excluir uma `timeOff` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="c22ad-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="c22ad-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c22ad-124">Properties</span></span>
|<span data-ttu-id="c22ad-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c22ad-125">Name</span></span>          |<span data-ttu-id="c22ad-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c22ad-126">Type</span></span>           |<span data-ttu-id="c22ad-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22ad-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c22ad-128">id</span><span class="sxs-lookup"><span data-stu-id="c22ad-128">id</span></span>            |`string`      |<span data-ttu-id="c22ad-129">A ID da tarefa `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="c22ad-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="c22ad-130">userId</span><span class="sxs-lookup"><span data-stu-id="c22ad-130">userId</span></span>            |`string`      |<span data-ttu-id="c22ad-131">ID do usuário atribuído ao `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="c22ad-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="c22ad-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c22ad-132">Required.</span></span>|
| <span data-ttu-id="c22ad-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-133">sharedTimeOff</span></span>     |[<span data-ttu-id="c22ad-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="c22ad-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="c22ad-135">A versão compartilhada desse `timeOff` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="c22ad-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="c22ad-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c22ad-136">Required.</span></span>|
| <span data-ttu-id="c22ad-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="c22ad-137">draftTimeOff</span></span>      |[<span data-ttu-id="c22ad-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="c22ad-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="c22ad-139">A versão de rascunho desse `timeOff` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="c22ad-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="c22ad-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c22ad-140">Required.</span></span>|
| <span data-ttu-id="c22ad-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c22ad-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="c22ad-142">O carimbo de data/hora `timeOff` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="c22ad-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="c22ad-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c22ad-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c22ad-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="c22ad-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c22ad-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c22ad-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="c22ad-146">O carimbo de data/hora `timeOff` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c22ad-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="c22ad-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c22ad-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c22ad-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="c22ad-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c22ad-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c22ad-149">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="c22ad-150">A identidade da última atualização `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="c22ad-150">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c22ad-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c22ad-151">JSON representation</span></span>

<span data-ttu-id="c22ad-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c22ad-152">Here is a JSON representation of the resource.</span></span>

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
