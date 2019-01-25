---
title: tipo de recurso de synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510551"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="f4fe8-103">tipo de recurso de synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f4fe8-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4fe8-104">Resume os resultados da execução do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="f4fe8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4fe8-105">Properties</span></span>
| <span data-ttu-id="f4fe8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4fe8-106">Property</span></span>     | <span data-ttu-id="f4fe8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4fe8-107">Type</span></span>   |<span data-ttu-id="f4fe8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fe8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4fe8-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4fe8-109">activityIdentifier</span></span>           |<span data-ttu-id="f4fe8-110">String</span><span class="sxs-lookup"><span data-stu-id="f4fe8-110">String</span></span> |<span data-ttu-id="f4fe8-111">Identificador da execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="f4fe8-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="f4fe8-112">countEntitled</span></span>                |<span data-ttu-id="f4fe8-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-113">Int64</span></span>  |<span data-ttu-id="f4fe8-114">Contagem de entradas processadas que foram atribuídas para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="f4fe8-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="f4fe8-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="f4fe8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-116">Int64</span></span>  |<span data-ttu-id="f4fe8-117">Contagem de entradas processadas que foram atribuídas pelo provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="f4fe8-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="f4fe8-118">countEscrowed</span></span>                |<span data-ttu-id="f4fe8-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-119">Int64</span></span>  |<span data-ttu-id="f4fe8-120">Contagem de entradas que foram caucionados (erros).</span><span class="sxs-lookup"><span data-stu-id="f4fe8-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="f4fe8-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="f4fe8-121">countEscrowedRaw</span></span>             |<span data-ttu-id="f4fe8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-122">Int64</span></span>  |<span data-ttu-id="f4fe8-123">Contagem de entradas que foram caucionadas, incluindo escrows gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="f4fe8-124">countExported</span><span class="sxs-lookup"><span data-stu-id="f4fe8-124">countExported</span></span>                |<span data-ttu-id="f4fe8-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-125">Int64</span></span>  |<span data-ttu-id="f4fe8-126">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-126">Count of exported entries.</span></span>|
|<span data-ttu-id="f4fe8-127">countExports</span><span class="sxs-lookup"><span data-stu-id="f4fe8-127">countExports</span></span>                 |<span data-ttu-id="f4fe8-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-128">Int64</span></span>  |<span data-ttu-id="f4fe8-129">Contagem de entradas que eram esperados a ser exportado.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="f4fe8-130">countImported</span><span class="sxs-lookup"><span data-stu-id="f4fe8-130">countImported</span></span>                |<span data-ttu-id="f4fe8-131">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-131">Int64</span></span>  |<span data-ttu-id="f4fe8-132">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-132">Count of imported entries.</span></span>|
|<span data-ttu-id="f4fe8-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="f4fe8-133">countImportedDeltas</span></span>          |<span data-ttu-id="f4fe8-134">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-134">Int64</span></span>  |<span data-ttu-id="f4fe8-135">Contagem de alterações de delta importadas.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="f4fe8-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="f4fe8-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="f4fe8-137">Int64</span><span class="sxs-lookup"><span data-stu-id="f4fe8-137">Int64</span></span>  |<span data-ttu-id="f4fe8-138">Contagem de alterações de delta importadas referentes às alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="f4fe8-139">erro</span><span class="sxs-lookup"><span data-stu-id="f4fe8-139">error</span></span>                        |[<span data-ttu-id="f4fe8-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="f4fe8-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="f4fe8-141">Se foi encontrado um erro, contém um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="f4fe8-142">estado</span><span class="sxs-lookup"><span data-stu-id="f4fe8-142">state</span></span>                        |<span data-ttu-id="f4fe8-143">String</span><span class="sxs-lookup"><span data-stu-id="f4fe8-143">String</span></span> |<span data-ttu-id="f4fe8-144">Resumindo o resultado dessa execução de código.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="f4fe8-145">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="f4fe8-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="f4fe8-146">timeBegan</span></span>                    |<span data-ttu-id="f4fe8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fe8-147">DateTimeOffset</span></span>|<span data-ttu-id="f4fe8-148">Começou a hora quando esse trabalho é executado.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-148">Time when this job run began.</span></span> <span data-ttu-id="f4fe8-149">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4fe8-150">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f4fe8-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="f4fe8-151">timeEnded</span></span>                    |<span data-ttu-id="f4fe8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fe8-152">DateTimeOffset</span></span>|<span data-ttu-id="f4fe8-153">Quando esse trabalho é executado de tempo é encerrada.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-153">Time when this job run ended.</span></span> <span data-ttu-id="f4fe8-154">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4fe8-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4fe8-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4fe8-156">JSON representation</span></span>

<span data-ttu-id="f4fe8-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4fe8-157">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
