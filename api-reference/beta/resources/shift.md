---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 16cce4d0c2ad6526154acd5895f5a24f76a7025d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520636"
---
# <a name="shift-resource-type"></a><span data-ttu-id="41cda-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="41cda-103">shift resource type</span></span>

<span data-ttu-id="41cda-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41cda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41cda-105">Uma unidade de trabalho agendado em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="41cda-105">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="41cda-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="41cda-106">Methods</span></span>

| <span data-ttu-id="41cda-107">Método</span><span class="sxs-lookup"><span data-stu-id="41cda-107">Method</span></span>       | <span data-ttu-id="41cda-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="41cda-108">Return Type</span></span>  |<span data-ttu-id="41cda-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="41cda-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41cda-110">Criar turno</span><span class="sxs-lookup"><span data-stu-id="41cda-110">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="41cda-111">desloca</span><span class="sxs-lookup"><span data-stu-id="41cda-111">shift</span></span>](shift.md) | <span data-ttu-id="41cda-112">Criar uma página `shift`.</span><span class="sxs-lookup"><span data-stu-id="41cda-112">Create a new `shift`.</span></span>|
|[<span data-ttu-id="41cda-113">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="41cda-113">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="41cda-114">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="41cda-114">[shift](shift.md) collection</span></span> | <span data-ttu-id="41cda-115">Obtenha a lista desse `shifts` cronograma.</span><span class="sxs-lookup"><span data-stu-id="41cda-115">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="41cda-116">Obter turno</span><span class="sxs-lookup"><span data-stu-id="41cda-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="41cda-117">desloca</span><span class="sxs-lookup"><span data-stu-id="41cda-117">shift</span></span>](shift.md) | <span data-ttu-id="41cda-118">Obter um `shift` por ID.</span><span class="sxs-lookup"><span data-stu-id="41cda-118">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="41cda-119">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="41cda-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="41cda-120">desloca</span><span class="sxs-lookup"><span data-stu-id="41cda-120">shift</span></span>](shift.md) | <span data-ttu-id="41cda-121">Substituir um `shift`.</span><span class="sxs-lookup"><span data-stu-id="41cda-121">Replace a `shift`.</span></span>|
|[<span data-ttu-id="41cda-122">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="41cda-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="41cda-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41cda-123">None</span></span> | <span data-ttu-id="41cda-124">Excluir uma `shift` do agendamento.</span><span class="sxs-lookup"><span data-stu-id="41cda-124">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="41cda-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41cda-125">Properties</span></span>
|<span data-ttu-id="41cda-126">Nome</span><span class="sxs-lookup"><span data-stu-id="41cda-126">Name</span></span>          |<span data-ttu-id="41cda-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="41cda-127">Type</span></span>           |<span data-ttu-id="41cda-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="41cda-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="41cda-129">id</span><span class="sxs-lookup"><span data-stu-id="41cda-129">id</span></span>            |`string`      |<span data-ttu-id="41cda-130">A ID da tarefa `shift`.</span><span class="sxs-lookup"><span data-stu-id="41cda-130">ID of the `shift`.</span></span>|
| <span data-ttu-id="41cda-131">userId</span><span class="sxs-lookup"><span data-stu-id="41cda-131">userId</span></span>            |`string`      |<span data-ttu-id="41cda-132">ID do usuário atribuído ao `shift`.</span><span class="sxs-lookup"><span data-stu-id="41cda-132">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="41cda-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cda-133">Required.</span></span> |
| <span data-ttu-id="41cda-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="41cda-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="41cda-135">ID do grupo de agendamento do `shift` qual o faz parte.</span><span class="sxs-lookup"><span data-stu-id="41cda-135">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="41cda-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cda-136">Required.</span></span> |
| <span data-ttu-id="41cda-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="41cda-137">sharedShift</span></span>   |[<span data-ttu-id="41cda-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="41cda-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="41cda-139">A versão compartilhada desse `shift` é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="41cda-139">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="41cda-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cda-140">Required.</span></span> |
| <span data-ttu-id="41cda-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="41cda-141">draftShift</span></span>        |[<span data-ttu-id="41cda-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="41cda-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="41cda-143">A versão de rascunho desse `shift` documento que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="41cda-143">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="41cda-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41cda-144">Required.</span></span> |
| <span data-ttu-id="41cda-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41cda-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="41cda-146">O carimbo de data/ `shift` hora em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="41cda-146">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="41cda-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41cda-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41cda-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="41cda-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="41cda-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41cda-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="41cda-150">O carimbo de data/ `shift` hora em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="41cda-150">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="41cda-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41cda-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41cda-152">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="41cda-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="41cda-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="41cda-153">lastModifiedBy</span></span>        | [<span data-ttu-id="41cda-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="41cda-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="41cda-155">A identidade da última atualização `shift`.</span><span class="sxs-lookup"><span data-stu-id="41cda-155">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41cda-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41cda-156">JSON representation</span></span>

<span data-ttu-id="41cda-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41cda-157">Here is a JSON representation of the resource.</span></span>

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
