---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657893"
---
# <a name="shift-resource-type"></a><span data-ttu-id="97f5e-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="97f5e-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97f5e-104">Uma unidade de trabalho agendado em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="97f5e-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="97f5e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="97f5e-105">Methods</span></span>

| <span data-ttu-id="97f5e-106">Método</span><span class="sxs-lookup"><span data-stu-id="97f5e-106">Method</span></span>       | <span data-ttu-id="97f5e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="97f5e-107">Return Type</span></span>  |<span data-ttu-id="97f5e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="97f5e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97f5e-109">Criar turno</span><span class="sxs-lookup"><span data-stu-id="97f5e-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="97f5e-110">desloca</span><span class="sxs-lookup"><span data-stu-id="97f5e-110">shift</span></span>](shift.md) | <span data-ttu-id="97f5e-111">Criar um novo `shift`.</span><span class="sxs-lookup"><span data-stu-id="97f5e-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="97f5e-112">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="97f5e-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="97f5e-113">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="97f5e-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="97f5e-114">Obtenha a lista desse `shifts` cronograma.</span><span class="sxs-lookup"><span data-stu-id="97f5e-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="97f5e-115">Obter turno</span><span class="sxs-lookup"><span data-stu-id="97f5e-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="97f5e-116">desloca</span><span class="sxs-lookup"><span data-stu-id="97f5e-116">shift</span></span>](shift.md) | <span data-ttu-id="97f5e-117">Obter a `shift` por ID.</span><span class="sxs-lookup"><span data-stu-id="97f5e-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="97f5e-118">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="97f5e-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="97f5e-119">desloca</span><span class="sxs-lookup"><span data-stu-id="97f5e-119">shift</span></span>](shift.md) | <span data-ttu-id="97f5e-120">Substitua um `shift`.</span><span class="sxs-lookup"><span data-stu-id="97f5e-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="97f5e-121">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="97f5e-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="97f5e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97f5e-122">None</span></span> | <span data-ttu-id="97f5e-123">Excluir uma `shift` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="97f5e-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="97f5e-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97f5e-124">Properties</span></span>
|<span data-ttu-id="97f5e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="97f5e-125">Name</span></span>          |<span data-ttu-id="97f5e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="97f5e-126">Type</span></span>           |<span data-ttu-id="97f5e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="97f5e-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="97f5e-128">id</span><span class="sxs-lookup"><span data-stu-id="97f5e-128">id</span></span>            |`string`      |<span data-ttu-id="97f5e-129">ID do `shift`.</span><span class="sxs-lookup"><span data-stu-id="97f5e-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="97f5e-130">userId</span><span class="sxs-lookup"><span data-stu-id="97f5e-130">userId</span></span>            |`string`      |<span data-ttu-id="97f5e-131">ID do usuário atribuído ao `shift`.</span><span class="sxs-lookup"><span data-stu-id="97f5e-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="97f5e-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97f5e-132">Required.</span></span> |
| <span data-ttu-id="97f5e-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="97f5e-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="97f5e-134">ID do grupo de agendamento do `shift` qual o faz parte.</span><span class="sxs-lookup"><span data-stu-id="97f5e-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="97f5e-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97f5e-135">Required.</span></span> |
| <span data-ttu-id="97f5e-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="97f5e-136">sharedShift</span></span>   |`[shiftItem](shiftitem.md)`  |<span data-ttu-id="97f5e-137">A versão compartilhada desse `shift` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="97f5e-137">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="97f5e-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97f5e-138">Required.</span></span> |
| <span data-ttu-id="97f5e-139">draftShift</span><span class="sxs-lookup"><span data-stu-id="97f5e-139">draftShift</span></span>        |`[shiftItem](shiftitem.md)`        |<span data-ttu-id="97f5e-140">A versão de rascunho desse `shift` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="97f5e-140">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="97f5e-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97f5e-141">Required.</span></span> |
| <span data-ttu-id="97f5e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97f5e-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="97f5e-143">O carimbo de data/ `shift` hora em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="97f5e-143">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="97f5e-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97f5e-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97f5e-145">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="97f5e-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="97f5e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97f5e-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="97f5e-147">O carimbo de data/ `shift` hora em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="97f5e-147">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="97f5e-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97f5e-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97f5e-149">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="97f5e-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="97f5e-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="97f5e-150">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="97f5e-151">A identidade que foi atualizada pela `shift`última vez.</span><span class="sxs-lookup"><span data-stu-id="97f5e-151">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97f5e-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97f5e-152">JSON representation</span></span>

<span data-ttu-id="97f5e-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97f5e-153">Here is a JSON representation of the resource.</span></span>

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
