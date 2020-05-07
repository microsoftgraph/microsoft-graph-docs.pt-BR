---
title: tipo de recurso Shift
description: Representa uma unidade de trabalho agendado no cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e38b8a000829ead91bdee28779a0f6988dd936ef
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154301"
---
# <a name="shift-resource-type"></a><span data-ttu-id="8d2b6-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="8d2b6-103">shift resource type</span></span>

<span data-ttu-id="8d2b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d2b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d2b6-105">Representa uma unidade de trabalho agendado em uma [agenda](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8d2b6-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8d2b6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d2b6-106">Methods</span></span>

| <span data-ttu-id="8d2b6-107">Método</span><span class="sxs-lookup"><span data-stu-id="8d2b6-107">Method</span></span>       | <span data-ttu-id="8d2b6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d2b6-108">Return Type</span></span>  |<span data-ttu-id="8d2b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d2b6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d2b6-110">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="8d2b6-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="8d2b6-111">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="8d2b6-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="8d2b6-112">Obtenha a lista de **turnos** neste cronograma.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="8d2b6-113">Criar turno</span><span class="sxs-lookup"><span data-stu-id="8d2b6-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="8d2b6-114">desloca</span><span class="sxs-lookup"><span data-stu-id="8d2b6-114">shift</span></span>](shift.md) | <span data-ttu-id="8d2b6-115">Criar um novo **turno**.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="8d2b6-116">Obter turno</span><span class="sxs-lookup"><span data-stu-id="8d2b6-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="8d2b6-117">desloca</span><span class="sxs-lookup"><span data-stu-id="8d2b6-117">shift</span></span>](shift.md) | <span data-ttu-id="8d2b6-118">Obter um **turno** por ID.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="8d2b6-119">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="8d2b6-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="8d2b6-120">desloca</span><span class="sxs-lookup"><span data-stu-id="8d2b6-120">shift</span></span>](shift.md) | <span data-ttu-id="8d2b6-121">Substitua um **Shift**.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="8d2b6-122">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="8d2b6-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="8d2b6-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d2b6-123">None</span></span> | <span data-ttu-id="8d2b6-124">Excluir uma **mudança** do cronograma.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d2b6-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d2b6-125">Properties</span></span>
|<span data-ttu-id="8d2b6-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8d2b6-126">Name</span></span>          |<span data-ttu-id="8d2b6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d2b6-127">Type</span></span>           |<span data-ttu-id="8d2b6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d2b6-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8d2b6-129">id</span><span class="sxs-lookup"><span data-stu-id="8d2b6-129">id</span></span>            |`string`      |<span data-ttu-id="8d2b6-130">ID do **turno**.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="8d2b6-131">userId</span><span class="sxs-lookup"><span data-stu-id="8d2b6-131">userId</span></span>            |`string`      |<span data-ttu-id="8d2b6-132">ID do usuário atribuído ao **turno**.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="8d2b6-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-133">Required.</span></span> |
| <span data-ttu-id="8d2b6-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="8d2b6-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="8d2b6-135">ID do grupo de agendamento do qual o **turno** faz parte.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="8d2b6-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-136">Required.</span></span> |
| <span data-ttu-id="8d2b6-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="8d2b6-137">sharedShift</span></span>   |[<span data-ttu-id="8d2b6-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8d2b6-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="8d2b6-139">A versão compartilhada dessa **mudança** que é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="8d2b6-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-140">Required.</span></span> |
| <span data-ttu-id="8d2b6-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="8d2b6-141">draftShift</span></span>        |[<span data-ttu-id="8d2b6-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8d2b6-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="8d2b6-143">A versão de rascunho desse **turno** que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="8d2b6-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-144">Required.</span></span> |
| <span data-ttu-id="8d2b6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2b6-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8d2b6-146">O carimbo de data/hora em que essa **mudança** foi criada pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="8d2b6-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d2b6-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8d2b6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2b6-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8d2b6-150">O carimbo de data/hora em que este **turno** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="8d2b6-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d2b6-152">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8d2b6-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8d2b6-153">lastModifiedBy</span></span>        | [<span data-ttu-id="8d2b6-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="8d2b6-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="8d2b6-155">A identidade que atualizou este **turno**pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d2b6-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d2b6-156">JSON representation</span></span>

<span data-ttu-id="8d2b6-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d2b6-157">The following is a JSON representation of the resource.</span></span>

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
