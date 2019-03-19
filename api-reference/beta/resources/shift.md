---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd80cd36bd32ea9efba9e565aabd2da963c51ec8
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676965"
---
# <a name="shift-resource-type"></a><span data-ttu-id="12ba9-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="12ba9-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12ba9-104">Uma unidade de trabalho agendado em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="12ba9-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="12ba9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="12ba9-105">Methods</span></span>

| <span data-ttu-id="12ba9-106">Método</span><span class="sxs-lookup"><span data-stu-id="12ba9-106">Method</span></span>       | <span data-ttu-id="12ba9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12ba9-107">Return Type</span></span>  |<span data-ttu-id="12ba9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ba9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12ba9-109">Criar turno</span><span class="sxs-lookup"><span data-stu-id="12ba9-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="12ba9-110">desloca</span><span class="sxs-lookup"><span data-stu-id="12ba9-110">shift</span></span>](shift.md) | <span data-ttu-id="12ba9-111">Criar um novo `shift`.</span><span class="sxs-lookup"><span data-stu-id="12ba9-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="12ba9-112">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="12ba9-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="12ba9-113">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="12ba9-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="12ba9-114">Obtenha a lista desse `shifts` cronograma.</span><span class="sxs-lookup"><span data-stu-id="12ba9-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="12ba9-115">Obter turno</span><span class="sxs-lookup"><span data-stu-id="12ba9-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="12ba9-116">desloca</span><span class="sxs-lookup"><span data-stu-id="12ba9-116">shift</span></span>](shift.md) | <span data-ttu-id="12ba9-117">Obter a `shift` por ID.</span><span class="sxs-lookup"><span data-stu-id="12ba9-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="12ba9-118">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="12ba9-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="12ba9-119">desloca</span><span class="sxs-lookup"><span data-stu-id="12ba9-119">shift</span></span>](shift.md) | <span data-ttu-id="12ba9-120">Substitua um `shift`.</span><span class="sxs-lookup"><span data-stu-id="12ba9-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="12ba9-121">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="12ba9-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="12ba9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12ba9-122">None</span></span> | <span data-ttu-id="12ba9-123">Excluir uma `shift` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="12ba9-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="12ba9-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12ba9-124">Properties</span></span>
|<span data-ttu-id="12ba9-125">Name</span><span class="sxs-lookup"><span data-stu-id="12ba9-125">Name</span></span>          |<span data-ttu-id="12ba9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="12ba9-126">Type</span></span>           |<span data-ttu-id="12ba9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ba9-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="12ba9-128">id</span><span class="sxs-lookup"><span data-stu-id="12ba9-128">id</span></span>            |`string`      |<span data-ttu-id="12ba9-129">ID do `shift`.</span><span class="sxs-lookup"><span data-stu-id="12ba9-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="12ba9-130">userId</span><span class="sxs-lookup"><span data-stu-id="12ba9-130">userId</span></span>            |`string`      |<span data-ttu-id="12ba9-131">ID do usuário atribuído ao `shift`.</span><span class="sxs-lookup"><span data-stu-id="12ba9-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="12ba9-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ba9-132">Required.</span></span> |
| <span data-ttu-id="12ba9-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="12ba9-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="12ba9-134">ID do grupo de agendamento do `shift` qual o faz parte.</span><span class="sxs-lookup"><span data-stu-id="12ba9-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="12ba9-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ba9-135">Required.</span></span> |
| <span data-ttu-id="12ba9-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="12ba9-136">sharedShift</span></span>   |[<span data-ttu-id="12ba9-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="12ba9-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="12ba9-138">A versão compartilhada desse `shift` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="12ba9-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="12ba9-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ba9-139">Required.</span></span> |
| <span data-ttu-id="12ba9-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="12ba9-140">draftShift</span></span>        |[<span data-ttu-id="12ba9-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="12ba9-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="12ba9-142">A versão de rascunho desse `shift` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="12ba9-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="12ba9-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ba9-143">Required.</span></span> |
| <span data-ttu-id="12ba9-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12ba9-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="12ba9-145">O carimbo de data/ `shift` hora em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="12ba9-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="12ba9-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12ba9-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12ba9-147">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="12ba9-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="12ba9-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12ba9-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="12ba9-149">O carimbo de data/ `shift` hora em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12ba9-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="12ba9-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12ba9-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12ba9-151">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="12ba9-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="12ba9-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="12ba9-152">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="12ba9-153">A identidade que foi atualizada pela `shift`última vez.</span><span class="sxs-lookup"><span data-stu-id="12ba9-153">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12ba9-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12ba9-154">JSON representation</span></span>

<span data-ttu-id="12ba9-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12ba9-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
