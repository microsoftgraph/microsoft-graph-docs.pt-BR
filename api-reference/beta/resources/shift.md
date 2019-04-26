---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f5c66d0f555ae6e5740883ed72964a8fa36df303
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343042"
---
# <a name="shift-resource-type"></a><span data-ttu-id="7a4dd-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="7a4dd-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a4dd-104">Uma unidade de trabalho agendado em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="7a4dd-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="7a4dd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7a4dd-105">Methods</span></span>

| <span data-ttu-id="7a4dd-106">Método</span><span class="sxs-lookup"><span data-stu-id="7a4dd-106">Method</span></span>       | <span data-ttu-id="7a4dd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7a4dd-107">Return Type</span></span>  |<span data-ttu-id="7a4dd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a4dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a4dd-109">Criar turno</span><span class="sxs-lookup"><span data-stu-id="7a4dd-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="7a4dd-110">desloca</span><span class="sxs-lookup"><span data-stu-id="7a4dd-110">shift</span></span>](shift.md) | <span data-ttu-id="7a4dd-111">Criar uma página `shift`.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="7a4dd-112">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="7a4dd-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="7a4dd-113">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="7a4dd-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="7a4dd-114">Obtenha a lista desse `shifts` cronograma.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="7a4dd-115">Obter turno</span><span class="sxs-lookup"><span data-stu-id="7a4dd-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="7a4dd-116">desloca</span><span class="sxs-lookup"><span data-stu-id="7a4dd-116">shift</span></span>](shift.md) | <span data-ttu-id="7a4dd-117">Obter um `shift` por ID.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="7a4dd-118">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="7a4dd-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="7a4dd-119">desloca</span><span class="sxs-lookup"><span data-stu-id="7a4dd-119">shift</span></span>](shift.md) | <span data-ttu-id="7a4dd-120">Substituir um `shift`.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="7a4dd-121">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="7a4dd-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="7a4dd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a4dd-122">None</span></span> | <span data-ttu-id="7a4dd-123">Excluir uma `shift` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a4dd-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a4dd-124">Properties</span></span>
|<span data-ttu-id="7a4dd-125">Nome</span><span class="sxs-lookup"><span data-stu-id="7a4dd-125">Name</span></span>          |<span data-ttu-id="7a4dd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a4dd-126">Type</span></span>           |<span data-ttu-id="7a4dd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a4dd-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7a4dd-128">id</span><span class="sxs-lookup"><span data-stu-id="7a4dd-128">id</span></span>            |`string`      |<span data-ttu-id="7a4dd-129">A ID da tarefa `shift`.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="7a4dd-130">userId</span><span class="sxs-lookup"><span data-stu-id="7a4dd-130">userId</span></span>            |`string`      |<span data-ttu-id="7a4dd-131">ID do usuário atribuído ao `shift`.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="7a4dd-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-132">Required.</span></span> |
| <span data-ttu-id="7a4dd-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="7a4dd-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="7a4dd-134">ID do grupo de agendamento do `shift` qual o faz parte.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="7a4dd-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-135">Required.</span></span> |
| <span data-ttu-id="7a4dd-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="7a4dd-136">sharedShift</span></span>   |[<span data-ttu-id="7a4dd-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="7a4dd-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="7a4dd-138">A versão compartilhada desse `shift` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="7a4dd-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-139">Required.</span></span> |
| <span data-ttu-id="7a4dd-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="7a4dd-140">draftShift</span></span>        |[<span data-ttu-id="7a4dd-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="7a4dd-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="7a4dd-142">A versão de rascunho desse `shift` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="7a4dd-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-143">Required.</span></span> |
| <span data-ttu-id="7a4dd-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4dd-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="7a4dd-145">O carimbo de data/ `shift` hora em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="7a4dd-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a4dd-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7a4dd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4dd-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="7a4dd-149">O carimbo de data/ `shift` hora em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="7a4dd-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a4dd-151">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7a4dd-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7a4dd-152">lastModifiedBy</span></span>        | [<span data-ttu-id="7a4dd-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="7a4dd-153">identitySet</span></span>](identityset.md)        |<span data-ttu-id="7a4dd-154">A identidade da última atualização `shift`.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-154">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a4dd-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a4dd-155">JSON representation</span></span>

<span data-ttu-id="7a4dd-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a4dd-156">Here is a JSON representation of the resource.</span></span>

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
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
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
  "suppressions": []
}
-->
