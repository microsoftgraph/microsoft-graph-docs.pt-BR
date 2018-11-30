---
title: tipo de recurso de synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036909"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="ac6a7-103">tipo de recurso de synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="ac6a7-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="ac6a7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac6a7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac6a7-106">Resume os resultados da execução do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="ac6a7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac6a7-107">Properties</span></span>
| <span data-ttu-id="ac6a7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac6a7-108">Property</span></span>     | <span data-ttu-id="ac6a7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac6a7-109">Type</span></span>   |<span data-ttu-id="ac6a7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac6a7-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac6a7-111">activityIdentifier</span></span>           |<span data-ttu-id="ac6a7-112">String</span><span class="sxs-lookup"><span data-stu-id="ac6a7-112">String</span></span> |<span data-ttu-id="ac6a7-113">Identificador da execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="ac6a7-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="ac6a7-114">countEntitled</span></span>                |<span data-ttu-id="ac6a7-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-115">Int64</span></span>  |<span data-ttu-id="ac6a7-116">Contagem de entradas processadas que foram atribuídas para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="ac6a7-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="ac6a7-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="ac6a7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-118">Int64</span></span>  |<span data-ttu-id="ac6a7-119">Contagem de entradas processadas que foram atribuídas pelo provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="ac6a7-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="ac6a7-120">countEscrowed</span></span>                |<span data-ttu-id="ac6a7-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-121">Int64</span></span>  |<span data-ttu-id="ac6a7-122">Contagem de entradas que foram caucionados (erros).</span><span class="sxs-lookup"><span data-stu-id="ac6a7-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="ac6a7-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="ac6a7-123">countEscrowedRaw</span></span>             |<span data-ttu-id="ac6a7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-124">Int64</span></span>  |<span data-ttu-id="ac6a7-125">Contagem de entradas que foram caucionadas, incluindo escrows gerada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="ac6a7-126">countExported</span><span class="sxs-lookup"><span data-stu-id="ac6a7-126">countExported</span></span>                |<span data-ttu-id="ac6a7-127">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-127">Int64</span></span>  |<span data-ttu-id="ac6a7-128">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-128">Count of exported entries.</span></span>|
|<span data-ttu-id="ac6a7-129">countExports</span><span class="sxs-lookup"><span data-stu-id="ac6a7-129">countExports</span></span>                 |<span data-ttu-id="ac6a7-130">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-130">Int64</span></span>  |<span data-ttu-id="ac6a7-131">Contagem de entradas que eram esperados a ser exportado.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="ac6a7-132">countImported</span><span class="sxs-lookup"><span data-stu-id="ac6a7-132">countImported</span></span>                |<span data-ttu-id="ac6a7-133">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-133">Int64</span></span>  |<span data-ttu-id="ac6a7-134">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-134">Count of imported entries.</span></span>|
|<span data-ttu-id="ac6a7-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="ac6a7-135">countImportedDeltas</span></span>          |<span data-ttu-id="ac6a7-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-136">Int64</span></span>  |<span data-ttu-id="ac6a7-137">Contagem de alterações de delta importadas.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="ac6a7-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="ac6a7-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="ac6a7-139">Int64</span><span class="sxs-lookup"><span data-stu-id="ac6a7-139">Int64</span></span>  |<span data-ttu-id="ac6a7-140">Contagem de alterações de delta importadas referentes às alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="ac6a7-141">erro</span><span class="sxs-lookup"><span data-stu-id="ac6a7-141">error</span></span>                        |[<span data-ttu-id="ac6a7-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="ac6a7-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="ac6a7-143">Se foi encontrado um erro, contém um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="ac6a7-144">state</span><span class="sxs-lookup"><span data-stu-id="ac6a7-144">state</span></span>                        |<span data-ttu-id="ac6a7-145">String</span><span class="sxs-lookup"><span data-stu-id="ac6a7-145">String</span></span> |<span data-ttu-id="ac6a7-146">Resumindo o resultado dessa execução de código.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="ac6a7-147">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="ac6a7-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="ac6a7-148">timeBegan</span></span>                    |<span data-ttu-id="ac6a7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6a7-149">DateTimeOffset</span></span>|<span data-ttu-id="ac6a7-150">Começou a hora quando esse trabalho é executado.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-150">Time when this job run began.</span></span> <span data-ttu-id="ac6a7-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac6a7-152">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ac6a7-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="ac6a7-153">timeEnded</span></span>                    |<span data-ttu-id="ac6a7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6a7-154">DateTimeOffset</span></span>|<span data-ttu-id="ac6a7-155">Quando esse trabalho é executado de tempo é encerrada.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-155">Time when this job run ended.</span></span> <span data-ttu-id="ac6a7-156">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac6a7-157">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac6a7-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac6a7-158">JSON representation</span></span>

<span data-ttu-id="ac6a7-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac6a7-159">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->