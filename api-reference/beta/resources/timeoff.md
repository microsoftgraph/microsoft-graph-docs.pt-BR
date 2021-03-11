---
title: Tipo de recurso timeOff
description: Uma unidade que não funciona na agenda.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9dc8d463e7015ffca2c2b49de503b9a0a3cb5709
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720197"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="86484-103">Tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="86484-103">timeOff resource type</span></span>

<span data-ttu-id="86484-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86484-105">Uma unidade que não funciona em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="86484-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="86484-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="86484-106">Methods</span></span>

| <span data-ttu-id="86484-107">Método</span><span class="sxs-lookup"><span data-stu-id="86484-107">Method</span></span>       | <span data-ttu-id="86484-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86484-108">Return Type</span></span>  |<span data-ttu-id="86484-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86484-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86484-110">Criar</span><span class="sxs-lookup"><span data-stu-id="86484-110">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="86484-111">timeOff</span><span class="sxs-lookup"><span data-stu-id="86484-111">timeOff</span></span>](timeoff.md) | <span data-ttu-id="86484-112">Crie um novo **objeto timeOff.**</span><span class="sxs-lookup"><span data-stu-id="86484-112">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="86484-113">List</span><span class="sxs-lookup"><span data-stu-id="86484-113">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="86484-114">[Coleção timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="86484-114">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="86484-115">Obter a lista de **objetos timeOff** nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="86484-115">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="86484-116">Get</span><span class="sxs-lookup"><span data-stu-id="86484-116">Get</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="86484-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="86484-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="86484-118">Obter um **objeto timeOff** por ID.</span><span class="sxs-lookup"><span data-stu-id="86484-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="86484-119">Replace</span><span class="sxs-lookup"><span data-stu-id="86484-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="86484-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="86484-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="86484-121">Substitua um **objeto timeOff.**</span><span class="sxs-lookup"><span data-stu-id="86484-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="86484-122">Delete</span><span class="sxs-lookup"><span data-stu-id="86484-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="86484-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="86484-123">None</span></span> | <span data-ttu-id="86484-124">**Exclua um objeto timeOff** da agenda.</span><span class="sxs-lookup"><span data-stu-id="86484-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="86484-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86484-125">Properties</span></span>
|<span data-ttu-id="86484-126">Nome</span><span class="sxs-lookup"><span data-stu-id="86484-126">Name</span></span>          |<span data-ttu-id="86484-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="86484-127">Type</span></span>           |<span data-ttu-id="86484-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="86484-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="86484-129">id</span><span class="sxs-lookup"><span data-stu-id="86484-129">id</span></span>            |`string`      |<span data-ttu-id="86484-130">A ID da tarefa `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="86484-130">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="86484-131">userId</span><span class="sxs-lookup"><span data-stu-id="86484-131">userId</span></span>            |`string`      |<span data-ttu-id="86484-132">ID do usuário atribuído ao `timeOff` .</span><span class="sxs-lookup"><span data-stu-id="86484-132">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="86484-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86484-133">Required.</span></span>|
| <span data-ttu-id="86484-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="86484-134">sharedTimeOff</span></span>     | [<span data-ttu-id="86484-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="86484-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="86484-136">A versão compartilhada disso `timeOff` que pode ser visualizada por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="86484-136">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="86484-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86484-137">Required.</span></span>|
| <span data-ttu-id="86484-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="86484-138">draftTimeOff</span></span>      | [<span data-ttu-id="86484-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="86484-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="86484-140">A versão de rascunho disso `timeOff` que pode ser visualizada pelos gerentes.</span><span class="sxs-lookup"><span data-stu-id="86484-140">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="86484-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86484-141">Required.</span></span>|
| <span data-ttu-id="86484-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86484-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="86484-143">O carimbo de data/hora no `timeOff` qual isso foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="86484-143">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="86484-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86484-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86484-145">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="86484-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="86484-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86484-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="86484-147">O carimbo de data/hora em que `timeOff` isso foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="86484-147">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="86484-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86484-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86484-149">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="86484-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="86484-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="86484-150">lastModifiedBy</span></span>        | [<span data-ttu-id="86484-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="86484-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="86484-152">A identidade da última atualização `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="86484-152">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86484-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86484-153">JSON representation</span></span>

<span data-ttu-id="86484-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86484-154">Here is a JSON representation of the resource.</span></span>

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


