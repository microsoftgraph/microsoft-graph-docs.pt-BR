---
title: tipo de recurso synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d777a575290699c2a936902614aa8ef0e8b042d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094908"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="fa142-103">tipo de recurso synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="fa142-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="fa142-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa142-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa142-105">Resume os resultados da execução do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fa142-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="fa142-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa142-106">Properties</span></span>
| <span data-ttu-id="fa142-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa142-107">Property</span></span>     | <span data-ttu-id="fa142-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa142-108">Type</span></span>   |<span data-ttu-id="fa142-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa142-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa142-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="fa142-110">activityIdentifier</span></span>           |<span data-ttu-id="fa142-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa142-111">String</span></span> |<span data-ttu-id="fa142-112">Identificador do trabalho executado.</span><span class="sxs-lookup"><span data-stu-id="fa142-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="fa142-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="fa142-113">countEntitled</span></span>                |<span data-ttu-id="fa142-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-114">Int64</span></span>  |<span data-ttu-id="fa142-115">Contagem de entradas processadas que foram atribuídas para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fa142-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="fa142-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="fa142-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="fa142-117">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-117">Int64</span></span>  |<span data-ttu-id="fa142-118">Contagem de entradas processadas que foram atribuídas para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="fa142-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="fa142-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="fa142-119">countEscrowed</span></span>                |<span data-ttu-id="fa142-120">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-120">Int64</span></span>  |<span data-ttu-id="fa142-121">Contagem de entradas que foram caução (erros).</span><span class="sxs-lookup"><span data-stu-id="fa142-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="fa142-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="fa142-122">countEscrowedRaw</span></span>             |<span data-ttu-id="fa142-123">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-123">Int64</span></span>  |<span data-ttu-id="fa142-124">Contagem de entradas que foram caução, incluindo caução geradas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="fa142-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="fa142-125">countExported</span><span class="sxs-lookup"><span data-stu-id="fa142-125">countExported</span></span>                |<span data-ttu-id="fa142-126">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-126">Int64</span></span>  |<span data-ttu-id="fa142-127">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="fa142-127">Count of exported entries.</span></span>|
|<span data-ttu-id="fa142-128">countExports</span><span class="sxs-lookup"><span data-stu-id="fa142-128">countExports</span></span>                 |<span data-ttu-id="fa142-129">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-129">Int64</span></span>  |<span data-ttu-id="fa142-130">Contagem de entradas que devem ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="fa142-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="fa142-131">countImported</span><span class="sxs-lookup"><span data-stu-id="fa142-131">countImported</span></span>                |<span data-ttu-id="fa142-132">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-132">Int64</span></span>  |<span data-ttu-id="fa142-133">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="fa142-133">Count of imported entries.</span></span>|
|<span data-ttu-id="fa142-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="fa142-134">countImportedDeltas</span></span>          |<span data-ttu-id="fa142-135">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-135">Int64</span></span>  |<span data-ttu-id="fa142-136">Contagem de alterações delta importadas.</span><span class="sxs-lookup"><span data-stu-id="fa142-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="fa142-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="fa142-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="fa142-138">Int64</span><span class="sxs-lookup"><span data-stu-id="fa142-138">Int64</span></span>  |<span data-ttu-id="fa142-139">Contagem de alterações delta importadas referentes a alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="fa142-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="fa142-140">erro</span><span class="sxs-lookup"><span data-stu-id="fa142-140">error</span></span>                        |[<span data-ttu-id="fa142-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="fa142-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="fa142-142">Se for encontrado um erro, conterá um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="fa142-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="fa142-143">state</span><span class="sxs-lookup"><span data-stu-id="fa142-143">state</span></span>                        |<span data-ttu-id="fa142-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa142-144">String</span></span> |<span data-ttu-id="fa142-145">Código que resume o resultado desta execução.</span><span class="sxs-lookup"><span data-stu-id="fa142-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="fa142-146">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="fa142-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="fa142-147">timecomeçou</span><span class="sxs-lookup"><span data-stu-id="fa142-147">timeBegan</span></span>                    |<span data-ttu-id="fa142-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa142-148">DateTimeOffset</span></span>|<span data-ttu-id="fa142-149">Hora em que esta execução de trabalho começou.</span><span class="sxs-lookup"><span data-stu-id="fa142-149">Time when this job run began.</span></span> <span data-ttu-id="fa142-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fa142-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa142-151">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa142-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="fa142-152">timeterminou</span><span class="sxs-lookup"><span data-stu-id="fa142-152">timeEnded</span></span>                    |<span data-ttu-id="fa142-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa142-153">DateTimeOffset</span></span>|<span data-ttu-id="fa142-154">Hora em que esse trabalho foi executado.</span><span class="sxs-lookup"><span data-stu-id="fa142-154">Time when this job run ended.</span></span> <span data-ttu-id="fa142-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fa142-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa142-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa142-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa142-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa142-157">JSON representation</span></span>

<span data-ttu-id="fa142-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa142-158">The following is a JSON representation of the resource.</span></span>

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


