---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 508ace24bc15eda6f722153d4e55f12699c461bb
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153741"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="13e3c-103">tipo de recurso timeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-103">timeOff resource type</span></span>

<span data-ttu-id="13e3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13e3c-105">Uma unidade de não funcionar em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="13e3c-105">A unit of non-work in a schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="13e3c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="13e3c-106">Methods</span></span>

| <span data-ttu-id="13e3c-107">Método</span><span class="sxs-lookup"><span data-stu-id="13e3c-107">Method</span></span>       | <span data-ttu-id="13e3c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13e3c-108">Return Type</span></span>  |<span data-ttu-id="13e3c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e3c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13e3c-110">List</span><span class="sxs-lookup"><span data-stu-id="13e3c-110">List</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="13e3c-111">coleção [timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="13e3c-111">[timeOff](timeoff.md) collection</span></span> | <span data-ttu-id="13e3c-112">Obtenha a lista de objetos **timeOff** neste cronograma.</span><span class="sxs-lookup"><span data-stu-id="13e3c-112">Get the list of **timeOff** objects in this schedule.</span></span>|
|[<span data-ttu-id="13e3c-113">Create</span><span class="sxs-lookup"><span data-stu-id="13e3c-113">Create</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="13e3c-114">timeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-114">timeOff</span></span>](timeoff.md) | <span data-ttu-id="13e3c-115">Criar um novo objeto **timeOff** .</span><span class="sxs-lookup"><span data-stu-id="13e3c-115">Create a new **timeOff** object.</span></span>|
|[<span data-ttu-id="13e3c-116">Get</span><span class="sxs-lookup"><span data-stu-id="13e3c-116">Get</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="13e3c-117">timeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-117">timeOff</span></span>](timeoff.md) | <span data-ttu-id="13e3c-118">Obtenha um objeto **timeOff** por ID.</span><span class="sxs-lookup"><span data-stu-id="13e3c-118">Get a **timeOff** object by ID.</span></span>|
|[<span data-ttu-id="13e3c-119">Replace</span><span class="sxs-lookup"><span data-stu-id="13e3c-119">Replace</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="13e3c-120">timeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-120">timeOff</span></span>](timeoff.md) | <span data-ttu-id="13e3c-121">Substituir um objeto **timeOff** .</span><span class="sxs-lookup"><span data-stu-id="13e3c-121">Replace a **timeOff** object.</span></span>|
|[<span data-ttu-id="13e3c-122">Delete</span><span class="sxs-lookup"><span data-stu-id="13e3c-122">Delete</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="13e3c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13e3c-123">None</span></span> | <span data-ttu-id="13e3c-124">Excluir um objeto **timeOff** da agenda.</span><span class="sxs-lookup"><span data-stu-id="13e3c-124">Delete a **timeOff** object from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="13e3c-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13e3c-125">Properties</span></span>
|<span data-ttu-id="13e3c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="13e3c-126">Name</span></span>          |<span data-ttu-id="13e3c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="13e3c-127">Type</span></span>           |<span data-ttu-id="13e3c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e3c-128">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="13e3c-129">id</span><span class="sxs-lookup"><span data-stu-id="13e3c-129">id</span></span>            |`string`      |<span data-ttu-id="13e3c-130">ID do **timeOff**.</span><span class="sxs-lookup"><span data-stu-id="13e3c-130">ID of the **timeOff**.</span></span>|
| <span data-ttu-id="13e3c-131">userId</span><span class="sxs-lookup"><span data-stu-id="13e3c-131">userId</span></span>            |`string`      |<span data-ttu-id="13e3c-132">ID do usuário atribuído ao **timeOff**.</span><span class="sxs-lookup"><span data-stu-id="13e3c-132">ID of the user assigned to the **timeOff**.</span></span> <span data-ttu-id="13e3c-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e3c-133">Required.</span></span>|
| <span data-ttu-id="13e3c-134">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-134">sharedTimeOff</span></span>     | [<span data-ttu-id="13e3c-135">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="13e3c-135">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="13e3c-136">A versão compartilhada desse **timeOff** que é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="13e3c-136">The shared version of this **timeOff** that is viewable by both employees and managers.</span></span> <span data-ttu-id="13e3c-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e3c-137">Required.</span></span>|
| <span data-ttu-id="13e3c-138">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="13e3c-138">draftTimeOff</span></span>      | [<span data-ttu-id="13e3c-139">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="13e3c-139">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="13e3c-140">A versão de rascunho desse **timeOff** que é visível por gerentes.</span><span class="sxs-lookup"><span data-stu-id="13e3c-140">The draft version of this **timeOff** that is viewable by managers.</span></span> <span data-ttu-id="13e3c-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e3c-141">Required.</span></span>|
| <span data-ttu-id="13e3c-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e3c-142">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="13e3c-143">O carimbo de data/hora em que este **timeOff** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="13e3c-143">The time stamp at which this **timeOff** was first created.</span></span> <span data-ttu-id="13e3c-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="13e3c-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13e3c-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="13e3c-145">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="13e3c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e3c-146">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="13e3c-147">O carimbo de data/hora em que este **timeOff** foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="13e3c-147">The time stamp at which this **timeOff** was last updated.</span></span> <span data-ttu-id="13e3c-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="13e3c-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13e3c-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="13e3c-149">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="13e3c-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="13e3c-150">lastModifiedBy</span></span>        | [<span data-ttu-id="13e3c-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="13e3c-151">identitySet</span></span>](identityset.md)        |<span data-ttu-id="13e3c-152">A identidade que atualizou pela última vez este **timeOff**.</span><span class="sxs-lookup"><span data-stu-id="13e3c-152">The identity that last updated this **timeOff**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13e3c-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13e3c-153">JSON representation</span></span>

<span data-ttu-id="13e3c-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13e3c-154">The following is a JSON representation of the resource.</span></span>

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
