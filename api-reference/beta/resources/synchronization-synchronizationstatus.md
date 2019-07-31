---
title: tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e99db38b4f6c925f7ec7bfb2345582d6f8f9dae1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964617"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="5fcd6-103">tipo de recurso synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="5fcd6-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fcd6-104">Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="5fcd6-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5fcd6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fcd6-105">Properties</span></span>

| <span data-ttu-id="5fcd6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fcd6-106">Property</span></span>                              | <span data-ttu-id="5fcd6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fcd6-107">Type</span></span>      | <span data-ttu-id="5fcd6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fcd6-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="5fcd6-109">código</span><span class="sxs-lookup"><span data-stu-id="5fcd6-109">code</span></span>|<span data-ttu-id="5fcd6-110">String</span><span class="sxs-lookup"><span data-stu-id="5fcd6-110">String</span></span>|<span data-ttu-id="5fcd6-111">Código de status de alto nível do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="5fcd6-112">Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="5fcd6-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="5fcd6-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="5fcd6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5fcd6-114">Int64</span></span>|<span data-ttu-id="5fcd6-115">Número de vezes consecutivas que esse trabalho falhou.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="5fcd6-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="5fcd6-116">escrowsPruned</span></span>|<span data-ttu-id="5fcd6-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fcd6-117">Boolean</span></span>|<span data-ttu-id="5fcd6-118">`true`Se as caução do trabalho (erros no nível do objeto) foram removidas durante a sincronização inicial.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="5fcd6-119">As caução podem ser removidas se durante a sincronização inicial, você atinge o limite de erros que normalmente colocam o trabalho em quarentena.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="5fcd6-120">Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="5fcd6-121">Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará que o cliente Limpe os erros.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="5fcd6-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="5fcd6-122">lastExecution</span></span>|[<span data-ttu-id="5fcd6-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5fcd6-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5fcd6-124">Detalhes da última execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="5fcd6-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="5fcd6-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="5fcd6-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5fcd6-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5fcd6-127">Detalhes da última execução deste trabalho, que não tinham erros.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="5fcd6-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="5fcd6-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="5fcd6-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5fcd6-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5fcd6-130">Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="5fcd6-131">progresso</span><span class="sxs-lookup"><span data-stu-id="5fcd6-131">progress</span></span>|<span data-ttu-id="5fcd6-132">coleção [synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="5fcd6-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="5fcd6-133">Detalhes do progresso de um trabalho para a conclusão.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="5fcd6-134">quarentena</span><span class="sxs-lookup"><span data-stu-id="5fcd6-134">quarantine</span></span>|[<span data-ttu-id="5fcd6-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="5fcd6-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="5fcd6-136">Se o trabalho estiver em quarentena, detalhes da quarentena.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="5fcd6-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="5fcd6-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="5fcd6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fcd6-138">DateTimeOffset</span></span>|<span data-ttu-id="5fcd6-139">O horário em que o estado Steady (não há mais alterações no processo) foi obtido pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="5fcd6-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fcd6-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5fcd6-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="5fcd6-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="5fcd6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fcd6-143">DateTimeOffset</span></span>|<span data-ttu-id="5fcd6-144">O horário em que o estado Steady (não mais alterações no processo) foi atingido pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="5fcd6-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fcd6-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5fcd6-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="5fcd6-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="5fcd6-148">coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5fcd6-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="5fcd6-149">Contagem de objetos sincronizados, listados por tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="5fcd6-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="5fcd6-150">troubleshootingUrl</span></span>|<span data-ttu-id="5fcd6-151">String</span><span class="sxs-lookup"><span data-stu-id="5fcd6-151">String</span></span>|<span data-ttu-id="5fcd6-152">No caso de um erro, a URL com as etapas de solução de problemas para o problema.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="5fcd6-153">Detalhes do código de status de sincronização</span><span class="sxs-lookup"><span data-stu-id="5fcd6-153">Synchronization status code details</span></span>

| <span data-ttu-id="5fcd6-154">Valor</span><span class="sxs-lookup"><span data-stu-id="5fcd6-154">Value</span></span>                              | <span data-ttu-id="5fcd6-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fcd6-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="5fcd6-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="5fcd6-156">NotConfigured</span></span>                       |<span data-ttu-id="5fcd6-157">O trabalho não foi configurado e nunca foi executado.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-157">Job was not configured and never run.</span></span> <span data-ttu-id="5fcd6-158">Nenhuma autorização foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-158">No authorization was provided.</span></span> |
|<span data-ttu-id="5fcd6-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="5fcd6-159">NotRun</span></span>                              |<span data-ttu-id="5fcd6-160">O trabalho foi configurado e possivelmente foi iniciado, mas não concluiu sua primeira execução.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="5fcd6-161">Ativo</span><span class="sxs-lookup"><span data-stu-id="5fcd6-161">Active</span></span>                              |<span data-ttu-id="5fcd6-162">O trabalho está sendo executado periodicamente.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-162">Job is running periodically.</span></span>|
|<span data-ttu-id="5fcd6-163">Em pausa</span><span class="sxs-lookup"><span data-stu-id="5fcd6-163">Paused</span></span>                              |<span data-ttu-id="5fcd6-164">O trabalho foi pausado (geralmente por um administrador) e não está em execução no momento, mas o estado do trabalho é preservado.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="5fcd6-165">Quarentena</span><span class="sxs-lookup"><span data-stu-id="5fcd6-165">Quarantine</span></span>                          |<span data-ttu-id="5fcd6-166">O trabalho está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-166">Job is in quarantine.</span></span> <span data-ttu-id="5fcd6-167">Isso pode acontecer quando há um alto volume de erros ou erros críticos, como credenciais revogadas/expiradas.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="5fcd6-168">Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com uma frequência reduzida.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fcd6-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fcd6-169">JSON representation</span></span>

<span data-ttu-id="5fcd6-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fcd6-170">The following is a JSON representation of the resource.</span></span>

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
