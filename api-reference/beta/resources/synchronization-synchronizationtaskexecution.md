---
title: Tipo de recurso synchronizationTaskExecution
description: Resume os resultados do trabalho de sincronização executado.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d83092949e1f27c9dac9744d2b4b16be4bcbae0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722045"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="9fd59-103">Tipo de recurso synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="9fd59-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="9fd59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fd59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd59-105">Resume os resultados do trabalho de sincronização executado.</span><span class="sxs-lookup"><span data-stu-id="9fd59-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="9fd59-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fd59-106">Properties</span></span>
| <span data-ttu-id="9fd59-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fd59-107">Property</span></span>     | <span data-ttu-id="9fd59-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd59-108">Type</span></span>   |<span data-ttu-id="9fd59-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd59-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fd59-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fd59-110">activityIdentifier</span></span>           |<span data-ttu-id="9fd59-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd59-111">String</span></span> |<span data-ttu-id="9fd59-112">Identificador do trabalho executado.</span><span class="sxs-lookup"><span data-stu-id="9fd59-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="9fd59-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="9fd59-113">countEntitled</span></span>                |<span data-ttu-id="9fd59-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-114">Int64</span></span>  |<span data-ttu-id="9fd59-115">Contagem de entradas processadas atribuídas a esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd59-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="9fd59-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="9fd59-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="9fd59-117">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-117">Int64</span></span>  |<span data-ttu-id="9fd59-118">Contagem de entradas processadas atribuídas ao provisionamento.</span><span class="sxs-lookup"><span data-stu-id="9fd59-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="9fd59-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="9fd59-119">countEscrowed</span></span>                |<span data-ttu-id="9fd59-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-120">Int64</span></span>  |<span data-ttu-id="9fd59-121">Contagem de entradas que foram escrotadas (erros).</span><span class="sxs-lookup"><span data-stu-id="9fd59-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="9fd59-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="9fd59-122">countEscrowedRaw</span></span>             |<span data-ttu-id="9fd59-123">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-123">Int64</span></span>  |<span data-ttu-id="9fd59-124">Contagem de entradas que foram escrotadas, incluindo escrows gerados pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="9fd59-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="9fd59-125">countExported</span><span class="sxs-lookup"><span data-stu-id="9fd59-125">countExported</span></span>                |<span data-ttu-id="9fd59-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-126">Int64</span></span>  |<span data-ttu-id="9fd59-127">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="9fd59-127">Count of exported entries.</span></span>|
|<span data-ttu-id="9fd59-128">countExports</span><span class="sxs-lookup"><span data-stu-id="9fd59-128">countExports</span></span>                 |<span data-ttu-id="9fd59-129">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-129">Int64</span></span>  |<span data-ttu-id="9fd59-130">Contagem de entradas que eram esperadas para serem exportadas.</span><span class="sxs-lookup"><span data-stu-id="9fd59-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="9fd59-131">countImported</span><span class="sxs-lookup"><span data-stu-id="9fd59-131">countImported</span></span>                |<span data-ttu-id="9fd59-132">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-132">Int64</span></span>  |<span data-ttu-id="9fd59-133">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="9fd59-133">Count of imported entries.</span></span>|
|<span data-ttu-id="9fd59-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="9fd59-134">countImportedDeltas</span></span>          |<span data-ttu-id="9fd59-135">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-135">Int64</span></span>  |<span data-ttu-id="9fd59-136">Contagem de alterações delta importadas.</span><span class="sxs-lookup"><span data-stu-id="9fd59-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="9fd59-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="9fd59-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="9fd59-138">Int64</span><span class="sxs-lookup"><span data-stu-id="9fd59-138">Int64</span></span>  |<span data-ttu-id="9fd59-139">Contagem de alterações delta importadas relacionadas a alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="9fd59-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="9fd59-140">erro</span><span class="sxs-lookup"><span data-stu-id="9fd59-140">error</span></span>                        |[<span data-ttu-id="9fd59-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="9fd59-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="9fd59-142">Se um erro foi encontrado, contém um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="9fd59-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="9fd59-143">estado</span><span class="sxs-lookup"><span data-stu-id="9fd59-143">state</span></span>                        |<span data-ttu-id="9fd59-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd59-144">String</span></span> |<span data-ttu-id="9fd59-145">Code summarizing the result of this run.</span><span class="sxs-lookup"><span data-stu-id="9fd59-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="9fd59-146">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="9fd59-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="9fd59-147">timeBegan</span><span class="sxs-lookup"><span data-stu-id="9fd59-147">timeBegan</span></span>                    |<span data-ttu-id="9fd59-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd59-148">DateTimeOffset</span></span>|<span data-ttu-id="9fd59-149">Hora em que esse trabalho foi executado.</span><span class="sxs-lookup"><span data-stu-id="9fd59-149">Time when this job run began.</span></span> <span data-ttu-id="9fd59-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9fd59-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fd59-151">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9fd59-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="9fd59-152">timeEnded</span><span class="sxs-lookup"><span data-stu-id="9fd59-152">timeEnded</span></span>                    |<span data-ttu-id="9fd59-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd59-153">DateTimeOffset</span></span>|<span data-ttu-id="9fd59-154">Hora em que esse trabalho foi executado.</span><span class="sxs-lookup"><span data-stu-id="9fd59-154">Time when this job run ended.</span></span> <span data-ttu-id="9fd59-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9fd59-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fd59-156">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9fd59-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fd59-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fd59-157">JSON representation</span></span>

<span data-ttu-id="9fd59-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd59-158">The following is a JSON representation of the resource.</span></span>

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


