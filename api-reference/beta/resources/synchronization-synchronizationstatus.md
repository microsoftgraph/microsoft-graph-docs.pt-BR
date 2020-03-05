---
title: tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179eda96e62c124de5c64688352040b62dfc6c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520027"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="2737c-103">tipo de recurso synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="2737c-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="2737c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2737c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2737c-105">Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="2737c-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2737c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2737c-106">Properties</span></span>

| <span data-ttu-id="2737c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2737c-107">Property</span></span>                              | <span data-ttu-id="2737c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2737c-108">Type</span></span>      | <span data-ttu-id="2737c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2737c-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="2737c-110">código</span><span class="sxs-lookup"><span data-stu-id="2737c-110">code</span></span>|<span data-ttu-id="2737c-111">String</span><span class="sxs-lookup"><span data-stu-id="2737c-111">String</span></span>|<span data-ttu-id="2737c-112">Código de status de alto nível do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2737c-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="2737c-113">Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="2737c-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="2737c-114">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="2737c-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="2737c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2737c-115">Int64</span></span>|<span data-ttu-id="2737c-116">Número de vezes consecutivas que esse trabalho falhou.</span><span class="sxs-lookup"><span data-stu-id="2737c-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="2737c-117">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="2737c-117">escrowsPruned</span></span>|<span data-ttu-id="2737c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2737c-118">Boolean</span></span>|<span data-ttu-id="2737c-119">`true`Se as caução do trabalho (erros no nível do objeto) foram removidas durante a sincronização inicial.</span><span class="sxs-lookup"><span data-stu-id="2737c-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="2737c-120">As caução podem ser removidas se durante a sincronização inicial, você atinge o limite de erros que normalmente colocam o trabalho em quarentena.</span><span class="sxs-lookup"><span data-stu-id="2737c-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="2737c-121">Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída.</span><span class="sxs-lookup"><span data-stu-id="2737c-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="2737c-122">Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará que o cliente Limpe os erros.</span><span class="sxs-lookup"><span data-stu-id="2737c-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="2737c-123">lastExecution</span><span class="sxs-lookup"><span data-stu-id="2737c-123">lastExecution</span></span>|[<span data-ttu-id="2737c-124">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="2737c-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="2737c-125">Detalhes da última execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="2737c-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="2737c-126">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="2737c-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="2737c-127">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="2737c-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="2737c-128">Detalhes da última execução deste trabalho, que não tinham erros.</span><span class="sxs-lookup"><span data-stu-id="2737c-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="2737c-129">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="2737c-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="2737c-130">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="2737c-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="2737c-131">Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="2737c-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="2737c-132">progresso</span><span class="sxs-lookup"><span data-stu-id="2737c-132">progress</span></span>|<span data-ttu-id="2737c-133">coleção [synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="2737c-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="2737c-134">Detalhes do progresso de um trabalho para a conclusão.</span><span class="sxs-lookup"><span data-stu-id="2737c-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="2737c-135">quarentena</span><span class="sxs-lookup"><span data-stu-id="2737c-135">quarantine</span></span>|[<span data-ttu-id="2737c-136">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="2737c-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="2737c-137">Se o trabalho estiver em quarentena, detalhes da quarentena.</span><span class="sxs-lookup"><span data-stu-id="2737c-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="2737c-138">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="2737c-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="2737c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2737c-139">DateTimeOffset</span></span>|<span data-ttu-id="2737c-140">O horário em que o estado Steady (não há mais alterações no processo) foi obtido pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="2737c-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="2737c-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2737c-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2737c-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2737c-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2737c-143">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="2737c-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="2737c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2737c-144">DateTimeOffset</span></span>|<span data-ttu-id="2737c-145">O horário em que o estado Steady (não mais alterações no processo) foi atingido pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2737c-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="2737c-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2737c-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2737c-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2737c-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2737c-148">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="2737c-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="2737c-149">coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2737c-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="2737c-150">Contagem de objetos sincronizados, listados por tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="2737c-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="2737c-151">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="2737c-151">troubleshootingUrl</span></span>|<span data-ttu-id="2737c-152">String</span><span class="sxs-lookup"><span data-stu-id="2737c-152">String</span></span>|<span data-ttu-id="2737c-153">No caso de um erro, a URL com as etapas de solução de problemas para o problema.</span><span class="sxs-lookup"><span data-stu-id="2737c-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="2737c-154">Detalhes do código de status de sincronização</span><span class="sxs-lookup"><span data-stu-id="2737c-154">Synchronization status code details</span></span>

| <span data-ttu-id="2737c-155">Valor</span><span class="sxs-lookup"><span data-stu-id="2737c-155">Value</span></span>                              | <span data-ttu-id="2737c-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="2737c-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="2737c-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="2737c-157">NotConfigured</span></span>                       |<span data-ttu-id="2737c-158">O trabalho não foi configurado e nunca foi executado.</span><span class="sxs-lookup"><span data-stu-id="2737c-158">Job was not configured and never run.</span></span> <span data-ttu-id="2737c-159">Nenhuma autorização foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="2737c-159">No authorization was provided.</span></span> |
|<span data-ttu-id="2737c-160">NotRun</span><span class="sxs-lookup"><span data-stu-id="2737c-160">NotRun</span></span>                              |<span data-ttu-id="2737c-161">O trabalho foi configurado e possivelmente foi iniciado, mas não concluiu sua primeira execução.</span><span class="sxs-lookup"><span data-stu-id="2737c-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="2737c-162">Ativo</span><span class="sxs-lookup"><span data-stu-id="2737c-162">Active</span></span>                              |<span data-ttu-id="2737c-163">O trabalho está sendo executado periodicamente.</span><span class="sxs-lookup"><span data-stu-id="2737c-163">Job is running periodically.</span></span>|
|<span data-ttu-id="2737c-164">Em pausa</span><span class="sxs-lookup"><span data-stu-id="2737c-164">Paused</span></span>                              |<span data-ttu-id="2737c-165">O trabalho foi pausado (geralmente por um administrador) e não está em execução no momento, mas o estado do trabalho é preservado.</span><span class="sxs-lookup"><span data-stu-id="2737c-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="2737c-166">Quarentena</span><span class="sxs-lookup"><span data-stu-id="2737c-166">Quarantine</span></span>                          |<span data-ttu-id="2737c-167">O trabalho está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="2737c-167">Job is in quarantine.</span></span> <span data-ttu-id="2737c-168">Isso pode acontecer quando há um alto volume de erros ou erros críticos, como credenciais revogadas/expiradas.</span><span class="sxs-lookup"><span data-stu-id="2737c-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="2737c-169">Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com uma frequência reduzida.</span><span class="sxs-lookup"><span data-stu-id="2737c-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2737c-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2737c-170">JSON representation</span></span>

<span data-ttu-id="2737c-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2737c-171">The following is a JSON representation of the resource.</span></span>

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
