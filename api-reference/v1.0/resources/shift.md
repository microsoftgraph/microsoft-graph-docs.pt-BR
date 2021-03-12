---
title: tipo de recurso shift
description: Representa uma unidade de trabalho agendada na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8c871e580818d96edcb0eae244c88c7edcc128c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721835"
---
# <a name="shift-resource-type"></a><span data-ttu-id="8e6c9-103">tipo de recurso shift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-103">shift resource type</span></span>

<span data-ttu-id="8e6c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e6c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e6c9-105">Representa uma unidade de trabalho agendada em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8e6c9-105">Represents a unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="8e6c9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8e6c9-106">Methods</span></span>

| <span data-ttu-id="8e6c9-107">Método</span><span class="sxs-lookup"><span data-stu-id="8e6c9-107">Method</span></span>       | <span data-ttu-id="8e6c9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e6c9-108">Return Type</span></span>  |<span data-ttu-id="8e6c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6c9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e6c9-110">Listar turnos</span><span class="sxs-lookup"><span data-stu-id="8e6c9-110">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="8e6c9-111">[coleção shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="8e6c9-111">[shift](shift.md) collection</span></span> | <span data-ttu-id="8e6c9-112">Obter a lista **de turnos** nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-112">Get the list of **shifts** in this schedule.</span></span>|
|[<span data-ttu-id="8e6c9-113">Criar turno</span><span class="sxs-lookup"><span data-stu-id="8e6c9-113">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="8e6c9-114">shift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-114">shift</span></span>](shift.md) | <span data-ttu-id="8e6c9-115">Criar um novo **turno**.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-115">Create a new **shift**.</span></span>|
|[<span data-ttu-id="8e6c9-116">Obter turno</span><span class="sxs-lookup"><span data-stu-id="8e6c9-116">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="8e6c9-117">shift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-117">shift</span></span>](shift.md) | <span data-ttu-id="8e6c9-118">Obter um **turno** por ID.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-118">Get a **shift** by ID.</span></span>|
|[<span data-ttu-id="8e6c9-119">Substituir turno</span><span class="sxs-lookup"><span data-stu-id="8e6c9-119">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="8e6c9-120">shift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-120">shift</span></span>](shift.md) | <span data-ttu-id="8e6c9-121">Substitua um **turno**.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-121">Replace a **shift**.</span></span>|
|[<span data-ttu-id="8e6c9-122">Excluir turno</span><span class="sxs-lookup"><span data-stu-id="8e6c9-122">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="8e6c9-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6c9-123">None</span></span> | <span data-ttu-id="8e6c9-124">**Exclua um turno** da agenda.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-124">Delete a **shift** from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e6c9-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e6c9-125">Properties</span></span>
|<span data-ttu-id="8e6c9-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8e6c9-126">Name</span></span>          |<span data-ttu-id="8e6c9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6c9-127">Type</span></span>           |<span data-ttu-id="8e6c9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6c9-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8e6c9-129">id</span><span class="sxs-lookup"><span data-stu-id="8e6c9-129">id</span></span>            |`string`      |<span data-ttu-id="8e6c9-130">ID do **turno**.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-130">ID of the **shift**.</span></span>|
| <span data-ttu-id="8e6c9-131">userId</span><span class="sxs-lookup"><span data-stu-id="8e6c9-131">userId</span></span>            |`string`      |<span data-ttu-id="8e6c9-132">ID do usuário atribuído ao **turno**.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-132">ID of the user assigned to the **shift**.</span></span> <span data-ttu-id="8e6c9-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-133">Required.</span></span> |
| <span data-ttu-id="8e6c9-134">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="8e6c9-134">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="8e6c9-135">A ID do grupo de agendamento **do turno** faz parte.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-135">ID of the scheduling group the **shift** is part of.</span></span> <span data-ttu-id="8e6c9-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-136">Required.</span></span> |
| <span data-ttu-id="8e6c9-137">sharedShift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-137">sharedShift</span></span>   |[<span data-ttu-id="8e6c9-138">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8e6c9-138">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="8e6c9-139">A versão compartilhada **dessa** mudança que pode ser visualizada por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-139">The shared version of this **shift** that is viewable by both employees and managers.</span></span> <span data-ttu-id="8e6c9-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-140">Required.</span></span> |
| <span data-ttu-id="8e6c9-141">draftShift</span><span class="sxs-lookup"><span data-stu-id="8e6c9-141">draftShift</span></span>        |[<span data-ttu-id="8e6c9-142">shiftItem</span><span class="sxs-lookup"><span data-stu-id="8e6c9-142">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="8e6c9-143">A versão de rascunho dessa **mudança** que pode ser visualizada pelos gerentes.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-143">The draft version of this **shift** that is viewable by managers.</span></span> <span data-ttu-id="8e6c9-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-144">Required.</span></span> |
| <span data-ttu-id="8e6c9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e6c9-145">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="8e6c9-146">O data/hora no qual esse **turno** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-146">The timestamp on which this **shift** was first created.</span></span> <span data-ttu-id="8e6c9-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e6c9-148">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8e6c9-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e6c9-149">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="8e6c9-150">O data/hora no qual esse **turno** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-150">The timestamp on which this **shift** was last updated.</span></span> <span data-ttu-id="8e6c9-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e6c9-152">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8e6c9-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8e6c9-153">lastModifiedBy</span></span>        | [<span data-ttu-id="8e6c9-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="8e6c9-154">identitySet</span></span>](identityset.md)        |<span data-ttu-id="8e6c9-155">A identidade que atualizou pela última vez esse **turno**.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-155">The identity that last updated this **shift**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e6c9-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e6c9-156">JSON representation</span></span>

<span data-ttu-id="8e6c9-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6c9-157">The following is a JSON representation of the resource.</span></span>

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

