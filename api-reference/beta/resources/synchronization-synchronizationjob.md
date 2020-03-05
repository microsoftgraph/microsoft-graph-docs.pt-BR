---
title: tipo de recurso synchronizationJob
description: Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cac54f10a3109be5596a62a84271a485a5f70449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520069"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="f5c4c-105">tipo de recurso synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f5c4c-105">synchronizationJob resource type</span></span>

<span data-ttu-id="f5c4c-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5c4c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c4c-107">Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-107">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="f5c4c-108">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-108">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="f5c4c-109">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-109">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="f5c4c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f5c4c-110">Methods</span></span>

| <span data-ttu-id="f5c4c-111">Método</span><span class="sxs-lookup"><span data-stu-id="f5c4c-111">Method</span></span>        | <span data-ttu-id="f5c4c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f5c4c-112">Return Type</span></span>               | <span data-ttu-id="f5c4c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c4c-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="f5c4c-114">List</span><span class="sxs-lookup"><span data-stu-id="f5c4c-114">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="f5c4c-115">coleção [synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-115">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="f5c4c-116">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="f5c4c-116">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="f5c4c-117">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f5c4c-117">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="f5c4c-118">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f5c4c-118">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="f5c4c-119">Ler propriedades e relações de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-119">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="f5c4c-120">Create</span><span class="sxs-lookup"><span data-stu-id="f5c4c-120">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="f5c4c-121">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f5c4c-121">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="f5c4c-122">Criar novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-122">Create new job for a given application.</span></span>|
|[<span data-ttu-id="f5c4c-123">Start</span><span class="sxs-lookup"><span data-stu-id="f5c4c-123">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="f5c4c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-124">None</span></span>   |<span data-ttu-id="f5c4c-125">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-125">Start synchronization.</span></span> <span data-ttu-id="f5c4c-126">Se o trabalho estiver em um estado pausado, ele continuará a partir do ponto em que o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-126">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="f5c4c-127">Se o trabalho estiver em quarentena, o status de quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-127">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="f5c4c-128">Restart</span><span class="sxs-lookup"><span data-stu-id="f5c4c-128">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="f5c4c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-129">None</span></span>   |<span data-ttu-id="f5c4c-130">Forçar o início do trabalho e processar novamente todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-130">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="f5c4c-131">Pause</span><span class="sxs-lookup"><span data-stu-id="f5c4c-131">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="f5c4c-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-132">None</span></span>   |<span data-ttu-id="f5c4c-133">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-133">Temporarily stop synchronization.</span></span> <span data-ttu-id="f5c4c-134">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-134">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="f5c4c-135">Delete</span><span class="sxs-lookup"><span data-stu-id="f5c4c-135">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="f5c4c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-136">None</span></span>   |<span data-ttu-id="f5c4c-137">Interrompa a sincronização e exclua permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-137">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="f5c4c-138">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f5c4c-138">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="f5c4c-139">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f5c4c-139">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="f5c4c-140">Recupere o esquema de sincronização efetiva do trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-140">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="f5c4c-141">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f5c4c-141">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="f5c4c-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-142">None</span></span>   |<span data-ttu-id="f5c4c-143">Atualize o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-143">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="f5c4c-144">Validar credenciais</span><span class="sxs-lookup"><span data-stu-id="f5c4c-144">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="f5c4c-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5c4c-145">None</span></span>|<span data-ttu-id="f5c4c-146">Teste as credenciais fornecidas em relação ao diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-146">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5c4c-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5c4c-147">Properties</span></span>

| <span data-ttu-id="f5c4c-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5c4c-148">Property</span></span>      | <span data-ttu-id="f5c4c-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5c4c-149">Type</span></span>      | <span data-ttu-id="f5c4c-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c4c-150">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f5c4c-151">id</span><span class="sxs-lookup"><span data-stu-id="f5c4c-151">id</span></span>             |<span data-ttu-id="f5c4c-152">String</span><span class="sxs-lookup"><span data-stu-id="f5c4c-152">String</span></span>                     |<span data-ttu-id="f5c4c-153">Identificador exclusivo do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-153">Unique synchronization job identifier.</span></span> <span data-ttu-id="f5c4c-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-154">Read-only.</span></span>|
|<span data-ttu-id="f5c4c-155">Cronograma</span><span class="sxs-lookup"><span data-stu-id="f5c4c-155">schedule</span></span>       |[<span data-ttu-id="f5c4c-156">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="f5c4c-156">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="f5c4c-157">Agendamento usado para executar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-157">Schedule used to run the job.</span></span> <span data-ttu-id="f5c4c-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-158">Read-only.</span></span>|
|<span data-ttu-id="f5c4c-159">status</span><span class="sxs-lookup"><span data-stu-id="f5c4c-159">status</span></span>         |[<span data-ttu-id="f5c4c-160">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="f5c4c-160">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="f5c4c-161">Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e os erros.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-161">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="f5c4c-162">synchronizationJobSettings</span><span class="sxs-lookup"><span data-stu-id="f5c4c-162">synchronizationJobSettings</span></span>   |[<span data-ttu-id="f5c4c-163">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="f5c4c-163">keyValuePair</span></span>](keyvaluepair.md)    |<span data-ttu-id="f5c4c-164">Configurações associadas ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-164">Settings associated with the job.</span></span> <span data-ttu-id="f5c4c-165">Algumas configurações são herdadas do modelo.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-165">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="f5c4c-166">templateId</span><span class="sxs-lookup"><span data-stu-id="f5c4c-166">templateId</span></span>     |<span data-ttu-id="f5c4c-167">String</span><span class="sxs-lookup"><span data-stu-id="f5c4c-167">String</span></span>    |<span data-ttu-id="f5c4c-168">Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que este trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-168">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5c4c-169">Relações</span><span class="sxs-lookup"><span data-stu-id="f5c4c-169">Relationships</span></span>
| <span data-ttu-id="f5c4c-170">Relação</span><span class="sxs-lookup"><span data-stu-id="f5c4c-170">Relationship</span></span> | <span data-ttu-id="f5c4c-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5c4c-171">Type</span></span>   |<span data-ttu-id="f5c4c-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c4c-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5c4c-173">esquemas</span><span class="sxs-lookup"><span data-stu-id="f5c4c-173">schema</span></span>|[<span data-ttu-id="f5c4c-174">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f5c4c-174">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="f5c4c-175">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-175">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5c4c-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5c4c-176">JSON representation</span></span>

<span data-ttu-id="f5c4c-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-177">The following is a JSON representation of the resource.</span></span>

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
