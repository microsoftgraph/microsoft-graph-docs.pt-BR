---
title: Tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 86320e6af31dae39f86ebe87f8490e24c7c33f57
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722052"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="7e048-103">Tipo de recurso synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="7e048-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="7e048-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e048-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e048-105">Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="7e048-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7e048-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e048-106">Properties</span></span>

| <span data-ttu-id="7e048-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e048-107">Property</span></span>                              | <span data-ttu-id="7e048-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e048-108">Type</span></span>      | <span data-ttu-id="7e048-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e048-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="7e048-110">código</span><span class="sxs-lookup"><span data-stu-id="7e048-110">code</span></span>|<span data-ttu-id="7e048-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e048-111">String</span></span>|<span data-ttu-id="7e048-112">Código de status de alto nível do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7e048-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="7e048-113">Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="7e048-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="7e048-114">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="7e048-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="7e048-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7e048-115">Int64</span></span>|<span data-ttu-id="7e048-116">Número de vezes consecutivas em que esse trabalho falhou.</span><span class="sxs-lookup"><span data-stu-id="7e048-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="7e048-117">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="7e048-117">escrowsPruned</span></span>|<span data-ttu-id="7e048-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e048-118">Boolean</span></span>|<span data-ttu-id="7e048-119">`true` se as escrows do trabalho (erros no nível do objeto) foram podadas durante a sincronização inicial.</span><span class="sxs-lookup"><span data-stu-id="7e048-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="7e048-120">Os escrows podem ser podados se, durante a sincronização inicial, você atingir o limite de erros que normalmente colocariam o trabalho em quarentena.</span><span class="sxs-lookup"><span data-stu-id="7e048-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="7e048-121">Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída.</span><span class="sxs-lookup"><span data-stu-id="7e048-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="7e048-122">Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará que o cliente limpe os erros.</span><span class="sxs-lookup"><span data-stu-id="7e048-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="7e048-123">lastExecution</span><span class="sxs-lookup"><span data-stu-id="7e048-123">lastExecution</span></span>|[<span data-ttu-id="7e048-124">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="7e048-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="7e048-125">Detalhes da última execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="7e048-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="7e048-126">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="7e048-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="7e048-127">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="7e048-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="7e048-128">Detalhes da última execução deste trabalho, que não teve erros.</span><span class="sxs-lookup"><span data-stu-id="7e048-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="7e048-129">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="7e048-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="7e048-130">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="7e048-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="7e048-131">Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="7e048-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="7e048-132">progresso</span><span class="sxs-lookup"><span data-stu-id="7e048-132">progress</span></span>|<span data-ttu-id="7e048-133">[Coleção synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="7e048-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="7e048-134">Detalhes do andamento de um trabalho para conclusão.</span><span class="sxs-lookup"><span data-stu-id="7e048-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="7e048-135">quarantine</span><span class="sxs-lookup"><span data-stu-id="7e048-135">quarantine</span></span>|[<span data-ttu-id="7e048-136">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="7e048-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="7e048-137">Se o trabalho estiver em quarentena, detalhes de quarentena.</span><span class="sxs-lookup"><span data-stu-id="7e048-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="7e048-138">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="7e048-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="7e048-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e048-139">DateTimeOffset</span></span>|<span data-ttu-id="7e048-140">O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="7e048-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="7e048-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7e048-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e048-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7e048-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="7e048-143">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="7e048-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="7e048-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e048-144">DateTimeOffset</span></span>|<span data-ttu-id="7e048-145">O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7e048-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="7e048-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7e048-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e048-147">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7e048-147">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="7e048-148">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="7e048-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="7e048-149">[coleção stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7e048-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="7e048-150">Contagem de objetos sincronizados, listados por tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="7e048-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="7e048-151">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="7e048-151">troubleshootingUrl</span></span>|<span data-ttu-id="7e048-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e048-152">String</span></span>|<span data-ttu-id="7e048-153">Em caso de erro, a URL com as etapas de solução de problemas para o problema.</span><span class="sxs-lookup"><span data-stu-id="7e048-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="7e048-154">Detalhes do código de status de sincronização</span><span class="sxs-lookup"><span data-stu-id="7e048-154">Synchronization status code details</span></span>

| <span data-ttu-id="7e048-155">Valor</span><span class="sxs-lookup"><span data-stu-id="7e048-155">Value</span></span>                              | <span data-ttu-id="7e048-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e048-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="7e048-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="7e048-157">NotConfigured</span></span>                       |<span data-ttu-id="7e048-158">O trabalho não foi configurado e nunca executado.</span><span class="sxs-lookup"><span data-stu-id="7e048-158">Job was not configured and never run.</span></span> <span data-ttu-id="7e048-159">Nenhuma autorização foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="7e048-159">No authorization was provided.</span></span> |
|<span data-ttu-id="7e048-160">NotRun</span><span class="sxs-lookup"><span data-stu-id="7e048-160">NotRun</span></span>                              |<span data-ttu-id="7e048-161">Job foi configurado e possivelmente iniciado, mas ainda não concluiu sua primeira executar.</span><span class="sxs-lookup"><span data-stu-id="7e048-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="7e048-162">Ativo</span><span class="sxs-lookup"><span data-stu-id="7e048-162">Active</span></span>                              |<span data-ttu-id="7e048-163">O trabalho é executado periodicamente.</span><span class="sxs-lookup"><span data-stu-id="7e048-163">Job is running periodically.</span></span>|
|<span data-ttu-id="7e048-164">Em pausa</span><span class="sxs-lookup"><span data-stu-id="7e048-164">Paused</span></span>                              |<span data-ttu-id="7e048-165">O trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.</span><span class="sxs-lookup"><span data-stu-id="7e048-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="7e048-166">Quarentena</span><span class="sxs-lookup"><span data-stu-id="7e048-166">Quarantine</span></span>                          |<span data-ttu-id="7e048-167">O trabalho está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="7e048-167">Job is in quarantine.</span></span> <span data-ttu-id="7e048-168">Isso pode acontecer quando houver um alto volume de erros ou erros críticos, como credenciais revogadas/expiradas.</span><span class="sxs-lookup"><span data-stu-id="7e048-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="7e048-169">Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com frequência reduzida.</span><span class="sxs-lookup"><span data-stu-id="7e048-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e048-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e048-170">JSON representation</span></span>

<span data-ttu-id="7e048-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e048-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


