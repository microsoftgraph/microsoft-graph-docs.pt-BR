---
title: tipo de recurso Shift
description: Representa uma unidade de trabalho agendado no cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52c83c8052725e99d1136df8b0c14d8d3c24ffe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086428"
---
# <a name="shift-resource-type"></a><span data-ttu-id="8bc4d-103">tipo de recurso Shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-103">shift resource type</span></span>

<span data-ttu-id="8bc4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bc4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8bc4d-105">Representa uma unidade de trabalho agendado em uma [agenda](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8bc4d-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8bc4d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8bc4d-106">Methods</span></span>

| <span data-ttu-id="8bc4d-107">Método</span><span class="sxs-lookup"><span data-stu-id="8bc4d-107">Method</span></span>       | <span data-ttu-id="8bc4d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8bc4d-108">Return Type</span></span>  |<span data-ttu-id="8bc4d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc4d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bc4d-110">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="8bc4d-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="8bc4d-111">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="8bc4d-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="8bc4d-112">Obtenha a lista de **turnos** neste cronograma.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="8bc4d-113">Criar turno</span><span class="sxs-lookup"><span data-stu-id="8bc4d-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="8bc4d-114">shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-114">shift</span></span>](shift.md) | <span data-ttu-id="8bc4d-115">Criar um novo **turno**.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="8bc4d-116">Obter turno</span><span class="sxs-lookup"><span data-stu-id="8bc4d-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="8bc4d-117">shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-117">shift</span></span>](shift.md) | <span data-ttu-id="8bc4d-118">Obter um **turno** por ID.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="8bc4d-119">Substituir Shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="8bc4d-120">shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-120">shift</span></span>](shift.md) | <span data-ttu-id="8bc4d-121">Substitua um **Shift**.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="8bc4d-122">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="8bc4d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8bc4d-123">None</span></span> | <span data-ttu-id="8bc4d-124">Excluir uma **mudança** do cronograma.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bc4d-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8bc4d-125">Properties</span></span>
|<span data-ttu-id="8bc4d-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8bc4d-126">Name</span></span>          |<span data-ttu-id="8bc4d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bc4d-127">Type</span></span>           |<span data-ttu-id="8bc4d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc4d-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8bc4d-129">id</span><span class="sxs-lookup"><span data-stu-id="8bc4d-129">id</span></span>            |`string`      |<span data-ttu-id="8bc4d-130">ID do **turno**.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="8bc4d-131">userId</span><span class="sxs-lookup"><span data-stu-id="8bc4d-131">userId</span></span>            |`string`      |<span data-ttu-id="8bc4d-132">ID do usuário atribuído ao **turno**.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="8bc4d-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-133">Required.</span></span> |
| <span data-ttu-id="8bc4d-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="8bc4d-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="8bc4d-135">ID do grupo de agendamento do qual o **turno** faz parte.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="8bc4d-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-136">Required.</span></span> |
| <span data-ttu-id="8bc4d-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-137">sharedShift</span></span>   |[<span data-ttu-id="8bc4d-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8bc4d-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="8bc4d-139">A versão compartilhada dessa **mudança** que é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="8bc4d-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-140">Required.</span></span> |
| <span data-ttu-id="8bc4d-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="8bc4d-141">draftShift</span></span>        |[<span data-ttu-id="8bc4d-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8bc4d-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="8bc4d-143">A versão de rascunho desse **turno** que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="8bc4d-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-144">Required.</span></span> |
| <span data-ttu-id="8bc4d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc4d-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8bc4d-146">O carimbo de data/hora em que essa **mudança** foi criada pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="8bc4d-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8bc4d-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8bc4d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc4d-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8bc4d-150">O carimbo de data/hora em que este **turno** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="8bc4d-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8bc4d-152">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-152">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="8bc4d-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8bc4d-153">lastModifiedBy</span></span>        | [<span data-ttu-id="8bc4d-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="8bc4d-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="8bc4d-155">A identidade que atualizou este **turno**pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bc4d-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8bc4d-156">JSON representation</span></span>

<span data-ttu-id="8bc4d-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8bc4d-157">The following is a JSON representation of the resource.</span></span>

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

