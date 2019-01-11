---
title: tipo de recurso de synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 01f30338d7f6d4388554df08bf91655136c24a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817028"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="bb999-103">tipo de recurso de synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="bb999-103">synchronizationStatus resource type</span></span>

> <span data-ttu-id="bb999-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb999-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb999-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb999-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb999-106">Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="bb999-106">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb999-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb999-107">Properties</span></span>

| <span data-ttu-id="bb999-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb999-108">Property</span></span>                              | <span data-ttu-id="bb999-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb999-109">Type</span></span>      | <span data-ttu-id="bb999-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb999-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="bb999-111">código</span><span class="sxs-lookup"><span data-stu-id="bb999-111">code</span></span>|<span data-ttu-id="bb999-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb999-112">String</span></span>|<span data-ttu-id="bb999-113">Código de alto nível de status do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="bb999-113">High-level status code of the synchronization job.</span></span> <span data-ttu-id="bb999-114">Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="bb999-114">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="bb999-115">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="bb999-115">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="bb999-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bb999-116">Int64</span></span>|<span data-ttu-id="bb999-117">Número de consecutivos vezes esse trabalho falhou.</span><span class="sxs-lookup"><span data-stu-id="bb999-117">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="bb999-118">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="bb999-118">escrowsPruned</span></span>|<span data-ttu-id="bb999-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb999-119">Boolean</span></span>|<span data-ttu-id="bb999-120">`true`Se escrows do trabalho (erros de nível de objeto) foram removidos durante a sincronização inicial.</span><span class="sxs-lookup"><span data-stu-id="bb999-120">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="bb999-121">Escrows podem ser removidos se durante a sincronização inicial, você atingir o limite de erros que faria normalmente para inserir o trabalho em quarentena.</span><span class="sxs-lookup"><span data-stu-id="bb999-121">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="bb999-122">Em vez de entrar em quarentena, o processo de sincronização limpa erros do trabalho e continua até que a sincronização inicial for concluída.</span><span class="sxs-lookup"><span data-stu-id="bb999-122">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="bb999-123">Quando a sincronização inicial for concluída, o trabalho será pausar e aguarde o cliente limpar os erros.</span><span class="sxs-lookup"><span data-stu-id="bb999-123">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="bb999-124">lastExecution</span><span class="sxs-lookup"><span data-stu-id="bb999-124">lastExecution</span></span>|[<span data-ttu-id="bb999-125">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="bb999-125">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="bb999-126">Detalhes da última execução do trabalho.</span><span class="sxs-lookup"><span data-stu-id="bb999-126">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="bb999-127">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="bb999-127">lastSuccessfulExecution</span></span>|[<span data-ttu-id="bb999-128">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="bb999-128">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="bb999-129">Detalhes da última execução do trabalho, que não teve que quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="bb999-129">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="bb999-130">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="bb999-130">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="bb999-131">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="bb999-131">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="bb999-132">Detalhes da última execução do trabalho, que são exportados de objetos para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="bb999-132">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="bb999-133">progresso</span><span class="sxs-lookup"><span data-stu-id="bb999-133">progress</span></span>|<span data-ttu-id="bb999-134">coleção [synchronizationProgress](synchronization-synchronizationprogress.md)</span><span class="sxs-lookup"><span data-stu-id="bb999-134">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="bb999-135">Detalhes do progresso de um trabalho de conclusão.</span><span class="sxs-lookup"><span data-stu-id="bb999-135">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="bb999-136">quarentena</span><span class="sxs-lookup"><span data-stu-id="bb999-136">quarantine</span></span>|[<span data-ttu-id="bb999-137">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="bb999-137">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="bb999-138">Se o trabalho estiver em quarentena, detalhes da quarentena.</span><span class="sxs-lookup"><span data-stu-id="bb999-138">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="bb999-139">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="bb999-139">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="bb999-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb999-140">DateTimeOffset</span></span>|<span data-ttu-id="bb999-141">A hora quando estável (sem alterações para o processo de mais) obteve pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="bb999-141">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="bb999-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bb999-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb999-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bb999-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bb999-144">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="bb999-144">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="bb999-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb999-145">DateTimeOffset</span></span>|<span data-ttu-id="bb999-146">A hora quando estável (sem alterações para o processo de mais) última obteve.</span><span class="sxs-lookup"><span data-stu-id="bb999-146">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="bb999-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bb999-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb999-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bb999-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bb999-149">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="bb999-149">synchronizedEntryCountByType</span></span>|<span data-ttu-id="bb999-150">coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bb999-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="bb999-151">Contagem de objetos sincronizados, listados por tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="bb999-151">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="bb999-152">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="bb999-152">troubleshootingUrl</span></span>|<span data-ttu-id="bb999-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb999-153">String</span></span>|<span data-ttu-id="bb999-154">Se ocorrer um erro, a URL com as etapas de solução de problemas para o problema.</span><span class="sxs-lookup"><span data-stu-id="bb999-154">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="bb999-155">Detalhes do código de status de sincronização</span><span class="sxs-lookup"><span data-stu-id="bb999-155">Synchronization status code details</span></span>

| <span data-ttu-id="bb999-156">Valor</span><span class="sxs-lookup"><span data-stu-id="bb999-156">Value</span></span>                              | <span data-ttu-id="bb999-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb999-157">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="bb999-158">Não-configuradas</span><span class="sxs-lookup"><span data-stu-id="bb999-158">NotConfigured</span></span>                       |<span data-ttu-id="bb999-159">Trabalho não foi configurado e nunca executar.</span><span class="sxs-lookup"><span data-stu-id="bb999-159">Job was not configured and never run.</span></span> <span data-ttu-id="bb999-160">Nenhuma autorização foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="bb999-160">No authorization was provided.</span></span> |
|<span data-ttu-id="bb999-161">NotRun</span><span class="sxs-lookup"><span data-stu-id="bb999-161">NotRun</span></span>                              |<span data-ttu-id="bb999-162">Trabalho tiver sido configurado e possivelmente iniciado, mas ainda não concluído sua primeira execução.</span><span class="sxs-lookup"><span data-stu-id="bb999-162">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="bb999-163">Ativo</span><span class="sxs-lookup"><span data-stu-id="bb999-163">Active</span></span>                              |<span data-ttu-id="bb999-164">Trabalho está sendo executado periodicamente.</span><span class="sxs-lookup"><span data-stu-id="bb999-164">Job is running periodically.</span></span>|
|<span data-ttu-id="bb999-165">Em pausa</span><span class="sxs-lookup"><span data-stu-id="bb999-165">Paused</span></span>                              |<span data-ttu-id="bb999-166">Trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.</span><span class="sxs-lookup"><span data-stu-id="bb999-166">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="bb999-167">Quarentena</span><span class="sxs-lookup"><span data-stu-id="bb999-167">Quarantine</span></span>                          |<span data-ttu-id="bb999-168">Trabalho está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="bb999-168">Job is in quarantine.</span></span> <span data-ttu-id="bb999-169">Isso pode acontecer quando há um alto volume de erros, ou erros críticos como credenciais revogado/expirou.</span><span class="sxs-lookup"><span data-stu-id="bb999-169">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="bb999-170">Enquanto em quarentena, o processo de sincronização tentar executar o trabalho com frequência reduzida.</span><span class="sxs-lookup"><span data-stu-id="bb999-170">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb999-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb999-171">JSON representation</span></span>

<span data-ttu-id="bb999-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb999-172">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
