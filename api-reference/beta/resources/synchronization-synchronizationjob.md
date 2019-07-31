---
title: tipo de recurso synchronizationJob
description: Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a311c8ae7618778c2dbd8cdbc9a5b30af254eae4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007792"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="66239-105">tipo de recurso synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="66239-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66239-106">Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="66239-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="66239-107">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="66239-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="66239-108">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="66239-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="66239-109">Methods</span></span>

| <span data-ttu-id="66239-110">Método</span><span class="sxs-lookup"><span data-stu-id="66239-110">Method</span></span>        | <span data-ttu-id="66239-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66239-111">Return Type</span></span>               | <span data-ttu-id="66239-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="66239-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="66239-113">List</span><span class="sxs-lookup"><span data-stu-id="66239-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="66239-114">coleção [synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="66239-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="66239-115">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="66239-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="66239-116">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="66239-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="66239-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="66239-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="66239-118">Ler propriedades e relações de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="66239-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="66239-119">Create</span><span class="sxs-lookup"><span data-stu-id="66239-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="66239-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="66239-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="66239-121">Criar novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66239-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="66239-122">Start</span><span class="sxs-lookup"><span data-stu-id="66239-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="66239-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-123">None</span></span>   |<span data-ttu-id="66239-124">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="66239-124">Start synchronization.</span></span> <span data-ttu-id="66239-125">Se o trabalho estiver em um estado pausado, ele continuará a partir do ponto em que o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="66239-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="66239-126">Se o trabalho estiver em quarentena, o status de quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="66239-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="66239-127">Restart</span><span class="sxs-lookup"><span data-stu-id="66239-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="66239-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-128">None</span></span>   |<span data-ttu-id="66239-129">Forçar o início do trabalho e processar novamente todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="66239-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="66239-130">Pause</span><span class="sxs-lookup"><span data-stu-id="66239-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="66239-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-131">None</span></span>   |<span data-ttu-id="66239-132">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="66239-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="66239-133">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="66239-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="66239-134">Delete</span><span class="sxs-lookup"><span data-stu-id="66239-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="66239-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-135">None</span></span>   |<span data-ttu-id="66239-136">Interrompa a sincronização e exclua permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="66239-137">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="66239-137">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="66239-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="66239-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="66239-139">Recupere o esquema de sincronização efetiva do trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="66239-140">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="66239-140">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="66239-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-141">None</span></span>   |<span data-ttu-id="66239-142">Atualize o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="66239-143">Validar credenciais</span><span class="sxs-lookup"><span data-stu-id="66239-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="66239-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66239-144">None</span></span>|<span data-ttu-id="66239-145">Teste as credenciais fornecidas em relação ao diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="66239-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="66239-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66239-146">Properties</span></span>

| <span data-ttu-id="66239-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66239-147">Property</span></span>      | <span data-ttu-id="66239-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="66239-148">Type</span></span>      | <span data-ttu-id="66239-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="66239-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="66239-150">id</span><span class="sxs-lookup"><span data-stu-id="66239-150">id</span></span>             |<span data-ttu-id="66239-151">String</span><span class="sxs-lookup"><span data-stu-id="66239-151">String</span></span>                     |<span data-ttu-id="66239-152">Identificador exclusivo do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="66239-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="66239-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66239-153">Read-only.</span></span>|
|<span data-ttu-id="66239-154">Cronograma</span><span class="sxs-lookup"><span data-stu-id="66239-154">schedule</span></span>       |[<span data-ttu-id="66239-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="66239-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="66239-156">Agendamento usado para executar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-156">Schedule used to run the job.</span></span> <span data-ttu-id="66239-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66239-157">Read-only.</span></span>|
|<span data-ttu-id="66239-158">status</span><span class="sxs-lookup"><span data-stu-id="66239-158">status</span></span>         |[<span data-ttu-id="66239-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="66239-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="66239-160">Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e os erros.</span><span class="sxs-lookup"><span data-stu-id="66239-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="66239-161">templateId</span><span class="sxs-lookup"><span data-stu-id="66239-161">templateId</span></span>     |<span data-ttu-id="66239-162">String</span><span class="sxs-lookup"><span data-stu-id="66239-162">String</span></span>    |<span data-ttu-id="66239-163">Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que este trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="66239-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66239-164">Relações</span><span class="sxs-lookup"><span data-stu-id="66239-164">Relationships</span></span>
| <span data-ttu-id="66239-165">Relação</span><span class="sxs-lookup"><span data-stu-id="66239-165">Relationship</span></span> | <span data-ttu-id="66239-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="66239-166">Type</span></span>   |<span data-ttu-id="66239-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="66239-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66239-168">esquemas</span><span class="sxs-lookup"><span data-stu-id="66239-168">schema</span></span>|[<span data-ttu-id="66239-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="66239-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="66239-170">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="66239-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66239-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66239-171">JSON representation</span></span>

<span data-ttu-id="66239-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66239-172">The following is a JSON representation of the resource.</span></span>

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
