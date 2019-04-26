---
title: tipo de recurso synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
ms.openlocfilehash: a9008dd7d51a1d07be75c5b9bbad34d636fff74c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339822"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="d69e1-103">tipo de recurso synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="d69e1-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d69e1-104">Resume os resultados da execução do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d69e1-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="d69e1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d69e1-105">Properties</span></span>
| <span data-ttu-id="d69e1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d69e1-106">Property</span></span>     | <span data-ttu-id="d69e1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d69e1-107">Type</span></span>   |<span data-ttu-id="d69e1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d69e1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d69e1-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d69e1-109">activityIdentifier</span></span>           |<span data-ttu-id="d69e1-110">String</span><span class="sxs-lookup"><span data-stu-id="d69e1-110">String</span></span> |<span data-ttu-id="d69e1-111">Identificador do trabalho executado.</span><span class="sxs-lookup"><span data-stu-id="d69e1-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="d69e1-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="d69e1-112">countEntitled</span></span>                |<span data-ttu-id="d69e1-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-113">Int64</span></span>  |<span data-ttu-id="d69e1-114">Contagem de entradas processadas que foram atribuídas para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d69e1-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="d69e1-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="d69e1-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="d69e1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-116">Int64</span></span>  |<span data-ttu-id="d69e1-117">Contagem de entradas processadas que foram atribuídas para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="d69e1-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="d69e1-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="d69e1-118">countEscrowed</span></span>                |<span data-ttu-id="d69e1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-119">Int64</span></span>  |<span data-ttu-id="d69e1-120">Contagem de entradas que foram caução (erros).</span><span class="sxs-lookup"><span data-stu-id="d69e1-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="d69e1-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="d69e1-121">countEscrowedRaw</span></span>             |<span data-ttu-id="d69e1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-122">Int64</span></span>  |<span data-ttu-id="d69e1-123">Contagem de entradas que foram caução, incluindo caução geradas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="d69e1-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="d69e1-124">countExported</span><span class="sxs-lookup"><span data-stu-id="d69e1-124">countExported</span></span>                |<span data-ttu-id="d69e1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-125">Int64</span></span>  |<span data-ttu-id="d69e1-126">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="d69e1-126">Count of exported entries.</span></span>|
|<span data-ttu-id="d69e1-127">countExports</span><span class="sxs-lookup"><span data-stu-id="d69e1-127">countExports</span></span>                 |<span data-ttu-id="d69e1-128">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-128">Int64</span></span>  |<span data-ttu-id="d69e1-129">Contagem de entradas que devem ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="d69e1-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="d69e1-130">countImported</span><span class="sxs-lookup"><span data-stu-id="d69e1-130">countImported</span></span>                |<span data-ttu-id="d69e1-131">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-131">Int64</span></span>  |<span data-ttu-id="d69e1-132">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="d69e1-132">Count of imported entries.</span></span>|
|<span data-ttu-id="d69e1-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="d69e1-133">countImportedDeltas</span></span>          |<span data-ttu-id="d69e1-134">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-134">Int64</span></span>  |<span data-ttu-id="d69e1-135">Contagem de alterações delta importadas.</span><span class="sxs-lookup"><span data-stu-id="d69e1-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="d69e1-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="d69e1-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="d69e1-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d69e1-137">Int64</span></span>  |<span data-ttu-id="d69e1-138">Contagem de alterações delta importadas referentes a alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="d69e1-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="d69e1-139">erro</span><span class="sxs-lookup"><span data-stu-id="d69e1-139">error</span></span>                        |[<span data-ttu-id="d69e1-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="d69e1-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="d69e1-141">Se for encontrado um erro, conterá um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="d69e1-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="d69e1-142">state</span><span class="sxs-lookup"><span data-stu-id="d69e1-142">state</span></span>                        |<span data-ttu-id="d69e1-143">String</span><span class="sxs-lookup"><span data-stu-id="d69e1-143">String</span></span> |<span data-ttu-id="d69e1-144">Código que resume o resultado desta execução.</span><span class="sxs-lookup"><span data-stu-id="d69e1-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="d69e1-145">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="d69e1-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="d69e1-146">timeComeçou</span><span class="sxs-lookup"><span data-stu-id="d69e1-146">timeBegan</span></span>                    |<span data-ttu-id="d69e1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d69e1-147">DateTimeOffset</span></span>|<span data-ttu-id="d69e1-148">Hora em que esta execução de trabalho começou.</span><span class="sxs-lookup"><span data-stu-id="d69e1-148">Time when this job run began.</span></span> <span data-ttu-id="d69e1-149">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d69e1-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d69e1-150">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d69e1-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d69e1-151">timeTerminou</span><span class="sxs-lookup"><span data-stu-id="d69e1-151">timeEnded</span></span>                    |<span data-ttu-id="d69e1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d69e1-152">DateTimeOffset</span></span>|<span data-ttu-id="d69e1-153">Hora em que esse trabalho foi executado.</span><span class="sxs-lookup"><span data-stu-id="d69e1-153">Time when this job run ended.</span></span> <span data-ttu-id="d69e1-154">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d69e1-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d69e1-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d69e1-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d69e1-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d69e1-156">JSON representation</span></span>

<span data-ttu-id="d69e1-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d69e1-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
