---
title: Tipo de recurso synchronizationJob
description: Executa a sincronização periodicamente em segundo plano, sondando alterações em um diretório e as pressionando para outro diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132038"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="0b853-103">Tipo de recurso synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0b853-103">synchronizationJob resource type</span></span>

<span data-ttu-id="0b853-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b853-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b853-105">Executa a sincronização periodicamente em segundo plano, sondando alterações em um diretório e fazendo com que elas para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="0b853-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="0b853-106">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="0b853-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="0b853-107">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="0b853-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b853-108">Methods</span></span>

| <span data-ttu-id="0b853-109">Método</span><span class="sxs-lookup"><span data-stu-id="0b853-109">Method</span></span>        | <span data-ttu-id="0b853-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b853-110">Return Type</span></span>               | <span data-ttu-id="0b853-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b853-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="0b853-112">List</span><span class="sxs-lookup"><span data-stu-id="0b853-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="0b853-113">[coleção synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="0b853-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="0b853-114">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="0b853-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="0b853-115">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0b853-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="0b853-116">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0b853-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="0b853-117">Ler propriedades e relações de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="0b853-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="0b853-118">Criar</span><span class="sxs-lookup"><span data-stu-id="0b853-118">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="0b853-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0b853-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="0b853-120">Crie um novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b853-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="0b853-121">Start</span><span class="sxs-lookup"><span data-stu-id="0b853-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="0b853-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-122">None</span></span>   |<span data-ttu-id="0b853-123">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b853-123">Start synchronization.</span></span> <span data-ttu-id="0b853-124">Se o trabalho estiver em um estado pausado, ele continuará do ponto em que o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="0b853-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="0b853-125">Se o trabalho estiver em quarentena, o status da quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="0b853-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="0b853-126">Restart</span><span class="sxs-lookup"><span data-stu-id="0b853-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="0b853-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-127">None</span></span>   |<span data-ttu-id="0b853-128">Force o trabalho a começar de novo e processe todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="0b853-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="0b853-129">Pause</span><span class="sxs-lookup"><span data-stu-id="0b853-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="0b853-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-130">None</span></span>   |<span data-ttu-id="0b853-131">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b853-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="0b853-132">Todo o progresso, incluindo o estado do trabalho, persiste, e o trabalho continuará de onde foi deixado quando [uma](../api/synchronization-synchronizationjob-start.md) chamada iniciar é feita.</span><span class="sxs-lookup"><span data-stu-id="0b853-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="0b853-133">Delete</span><span class="sxs-lookup"><span data-stu-id="0b853-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="0b853-134">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-134">None</span></span>   |<span data-ttu-id="0b853-135">Pare a sincronização e exclua permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="0b853-136">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0b853-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="0b853-137">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0b853-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="0b853-138">Recupere o esquema de sincronização eficaz do trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="0b853-139">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0b853-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="0b853-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-140">None</span></span>   |<span data-ttu-id="0b853-141">Atualize o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="0b853-142">Validar credenciais</span><span class="sxs-lookup"><span data-stu-id="0b853-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="0b853-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0b853-143">None</span></span>|<span data-ttu-id="0b853-144">Teste as credenciais fornecidas no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="0b853-144">Test provided credentials against target directory.</span></span>|
|[<span data-ttu-id="0b853-145">provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="0b853-145">provisionOnDemand</span></span>](../api/synchronization-synchronizationjob-provision-on-demand.md)|<span data-ttu-id="0b853-146">[Coleção synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="0b853-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="0b853-147">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="0b853-147">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="0b853-148">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="0b853-148">The resource is primarily used for on-demand provisioning.</span></span> |
## <a name="properties"></a><span data-ttu-id="0b853-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b853-149">Properties</span></span>

| <span data-ttu-id="0b853-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b853-150">Property</span></span>      | <span data-ttu-id="0b853-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b853-151">Type</span></span>      | <span data-ttu-id="0b853-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b853-152">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0b853-153">id</span><span class="sxs-lookup"><span data-stu-id="0b853-153">id</span></span>             |<span data-ttu-id="0b853-154">String</span><span class="sxs-lookup"><span data-stu-id="0b853-154">String</span></span>                     |<span data-ttu-id="0b853-155">Identificador exclusivo do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b853-155">Unique synchronization job identifier.</span></span> <span data-ttu-id="0b853-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b853-156">Read-only.</span></span>|
|<span data-ttu-id="0b853-157">Cronograma</span><span class="sxs-lookup"><span data-stu-id="0b853-157">schedule</span></span>       |[<span data-ttu-id="0b853-158">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="0b853-158">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="0b853-159">Agenda usada para executar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-159">Schedule used to run the job.</span></span> <span data-ttu-id="0b853-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b853-160">Read-only.</span></span>|
|<span data-ttu-id="0b853-161">status</span><span class="sxs-lookup"><span data-stu-id="0b853-161">status</span></span>         |[<span data-ttu-id="0b853-162">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="0b853-162">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="0b853-163">Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e erros.</span><span class="sxs-lookup"><span data-stu-id="0b853-163">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="0b853-164">synchronizationJobSettings</span><span class="sxs-lookup"><span data-stu-id="0b853-164">synchronizationJobSettings</span></span>   |[<span data-ttu-id="0b853-165">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="0b853-165">keyValuePair</span></span>](keyvaluepair.md)    |<span data-ttu-id="0b853-166">Configurações associadas ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-166">Settings associated with the job.</span></span> <span data-ttu-id="0b853-167">Algumas configurações são herdadas do modelo.</span><span class="sxs-lookup"><span data-stu-id="0b853-167">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="0b853-168">templateId</span><span class="sxs-lookup"><span data-stu-id="0b853-168">templateId</span></span>     |<span data-ttu-id="0b853-169">String</span><span class="sxs-lookup"><span data-stu-id="0b853-169">String</span></span>    |<span data-ttu-id="0b853-170">Identificador do modelo [de sincronização](synchronization-synchronizationtemplate.md) em que esse trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="0b853-170">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b853-171">Relações</span><span class="sxs-lookup"><span data-stu-id="0b853-171">Relationships</span></span>
| <span data-ttu-id="0b853-172">Relação</span><span class="sxs-lookup"><span data-stu-id="0b853-172">Relationship</span></span> | <span data-ttu-id="0b853-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b853-173">Type</span></span>   |<span data-ttu-id="0b853-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b853-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b853-175">schema</span><span class="sxs-lookup"><span data-stu-id="0b853-175">schema</span></span>|[<span data-ttu-id="0b853-176">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0b853-176">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="0b853-177">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b853-177">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b853-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b853-178">JSON representation</span></span>

<span data-ttu-id="0b853-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b853-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


