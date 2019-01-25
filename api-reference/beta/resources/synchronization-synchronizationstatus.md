---
title: tipo de recurso de synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523761"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="1c21c-103">tipo de recurso de synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="1c21c-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c21c-104">Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="1c21c-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1c21c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c21c-105">Properties</span></span>

| <span data-ttu-id="1c21c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c21c-106">Property</span></span>                              | <span data-ttu-id="1c21c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c21c-107">Type</span></span>      | <span data-ttu-id="1c21c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c21c-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="1c21c-109">código</span><span class="sxs-lookup"><span data-stu-id="1c21c-109">code</span></span>|<span data-ttu-id="1c21c-110">String</span><span class="sxs-lookup"><span data-stu-id="1c21c-110">String</span></span>|<span data-ttu-id="1c21c-111">Código de alto nível de status do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1c21c-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="1c21c-112">Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="1c21c-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="1c21c-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="1c21c-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="1c21c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1c21c-114">Int64</span></span>|<span data-ttu-id="1c21c-115">Número de consecutivos vezes esse trabalho falhou.</span><span class="sxs-lookup"><span data-stu-id="1c21c-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="1c21c-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="1c21c-116">escrowsPruned</span></span>|<span data-ttu-id="1c21c-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c21c-117">Boolean</span></span>|<span data-ttu-id="1c21c-118">`true`Se escrows do trabalho (erros de nível de objeto) foram removidos durante a sincronização inicial.</span><span class="sxs-lookup"><span data-stu-id="1c21c-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="1c21c-119">Escrows podem ser removidos se durante a sincronização inicial, você atingir o limite de erros que faria normalmente para inserir o trabalho em quarentena.</span><span class="sxs-lookup"><span data-stu-id="1c21c-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="1c21c-120">Em vez de entrar em quarentena, o processo de sincronização limpa erros do trabalho e continua até que a sincronização inicial for concluída.</span><span class="sxs-lookup"><span data-stu-id="1c21c-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="1c21c-121">Quando a sincronização inicial for concluída, o trabalho será pausar e aguarde o cliente limpar os erros.</span><span class="sxs-lookup"><span data-stu-id="1c21c-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="1c21c-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="1c21c-122">lastExecution</span></span>|[<span data-ttu-id="1c21c-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="1c21c-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="1c21c-124">Detalhes da última execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="1c21c-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="1c21c-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="1c21c-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="1c21c-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="1c21c-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="1c21c-127">Detalhes da última execução do trabalho, que não teve que quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="1c21c-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="1c21c-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="1c21c-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="1c21c-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="1c21c-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="1c21c-130">Detalhes da última execução do trabalho, que são exportados de objetos para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1c21c-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="1c21c-131">Progress</span><span class="sxs-lookup"><span data-stu-id="1c21c-131">progress</span></span>|<span data-ttu-id="1c21c-132">coleção [synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="1c21c-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="1c21c-133">Detalhes do progresso de um trabalho de conclusão.</span><span class="sxs-lookup"><span data-stu-id="1c21c-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="1c21c-134">quarentena</span><span class="sxs-lookup"><span data-stu-id="1c21c-134">quarantine</span></span>|[<span data-ttu-id="1c21c-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="1c21c-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="1c21c-136">Se o trabalho estiver em quarentena, detalhes da quarentena.</span><span class="sxs-lookup"><span data-stu-id="1c21c-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="1c21c-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="1c21c-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="1c21c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c21c-138">DateTimeOffset</span></span>|<span data-ttu-id="1c21c-139">A hora quando estável (sem alterações para o processo de mais) obteve pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="1c21c-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="1c21c-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1c21c-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c21c-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1c21c-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1c21c-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="1c21c-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="1c21c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c21c-143">DateTimeOffset</span></span>|<span data-ttu-id="1c21c-144">A hora quando estável (sem alterações para o processo de mais) última obteve.</span><span class="sxs-lookup"><span data-stu-id="1c21c-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="1c21c-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1c21c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c21c-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1c21c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1c21c-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="1c21c-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="1c21c-148">coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1c21c-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="1c21c-149">Contagem de objetos sincronizados, listados por tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="1c21c-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="1c21c-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="1c21c-150">troubleshootingUrl</span></span>|<span data-ttu-id="1c21c-151">String</span><span class="sxs-lookup"><span data-stu-id="1c21c-151">String</span></span>|<span data-ttu-id="1c21c-152">Se ocorrer um erro, a URL com as etapas de solução de problemas para o problema.</span><span class="sxs-lookup"><span data-stu-id="1c21c-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="1c21c-153">Detalhes do código de status de sincronização</span><span class="sxs-lookup"><span data-stu-id="1c21c-153">Synchronization status code details</span></span>

| <span data-ttu-id="1c21c-154">Valor</span><span class="sxs-lookup"><span data-stu-id="1c21c-154">Value</span></span>                              | <span data-ttu-id="1c21c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c21c-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="1c21c-156">Não-configuradas</span><span class="sxs-lookup"><span data-stu-id="1c21c-156">NotConfigured</span></span>                       |<span data-ttu-id="1c21c-157">Trabalho não foi configurado e nunca executar.</span><span class="sxs-lookup"><span data-stu-id="1c21c-157">Job was not configured and never run.</span></span> <span data-ttu-id="1c21c-158">Nenhuma autorização foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="1c21c-158">No authorization was provided.</span></span> |
|<span data-ttu-id="1c21c-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="1c21c-159">NotRun</span></span>                              |<span data-ttu-id="1c21c-160">Trabalho tiver sido configurado e possivelmente iniciado, mas ainda não concluído sua primeira execução.</span><span class="sxs-lookup"><span data-stu-id="1c21c-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="1c21c-161">Ativo</span><span class="sxs-lookup"><span data-stu-id="1c21c-161">Active</span></span>                              |<span data-ttu-id="1c21c-162">Trabalho está sendo executado periodicamente.</span><span class="sxs-lookup"><span data-stu-id="1c21c-162">Job is running periodically.</span></span>|
|<span data-ttu-id="1c21c-163">Em pausa</span><span class="sxs-lookup"><span data-stu-id="1c21c-163">Paused</span></span>                              |<span data-ttu-id="1c21c-164">Trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.</span><span class="sxs-lookup"><span data-stu-id="1c21c-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="1c21c-165">Quarentena</span><span class="sxs-lookup"><span data-stu-id="1c21c-165">Quarantine</span></span>                          |<span data-ttu-id="1c21c-166">Trabalho está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="1c21c-166">Job is in quarantine.</span></span> <span data-ttu-id="1c21c-167">Isso pode acontecer quando há um alto volume de erros, ou erros críticos como credenciais revogado/expirou.</span><span class="sxs-lookup"><span data-stu-id="1c21c-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="1c21c-168">Enquanto em quarentena, o processo de sincronização tentar executar o trabalho com frequência reduzida.</span><span class="sxs-lookup"><span data-stu-id="1c21c-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c21c-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c21c-169">JSON representation</span></span>

<span data-ttu-id="1c21c-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c21c-170">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
