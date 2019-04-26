---
title: tipo de recurso synchronizationJob
description: Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580656"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="7925d-105">tipo de recurso synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="7925d-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7925d-106">Realiza a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="7925d-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="7925d-107">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="7925d-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="7925d-108">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="7925d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7925d-109">Methods</span></span>

| <span data-ttu-id="7925d-110">Método</span><span class="sxs-lookup"><span data-stu-id="7925d-110">Method</span></span>        | <span data-ttu-id="7925d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7925d-111">Return Type</span></span>               | <span data-ttu-id="7925d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7925d-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="7925d-113">List</span><span class="sxs-lookup"><span data-stu-id="7925d-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="7925d-114">coleção [synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="7925d-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="7925d-115">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="7925d-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="7925d-116">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="7925d-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="7925d-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="7925d-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="7925d-118">Ler propriedades e relações de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="7925d-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="7925d-119">Create</span><span class="sxs-lookup"><span data-stu-id="7925d-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="7925d-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="7925d-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="7925d-121">Criar novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7925d-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="7925d-122">Start</span><span class="sxs-lookup"><span data-stu-id="7925d-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="7925d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-123">None</span></span>   |<span data-ttu-id="7925d-124">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="7925d-124">Start synchronization.</span></span> <span data-ttu-id="7925d-125">Se o trabalho estiver em um estado pausado, ele continuará a partir do ponto em que o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="7925d-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="7925d-126">Se o trabalho estiver em quarentena, o status de quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="7925d-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="7925d-127">Restart</span><span class="sxs-lookup"><span data-stu-id="7925d-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="7925d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-128">None</span></span>   |<span data-ttu-id="7925d-129">Forçar o início do trabalho e processar novamente todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="7925d-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="7925d-130">Pause</span><span class="sxs-lookup"><span data-stu-id="7925d-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="7925d-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-131">None</span></span>   |<span data-ttu-id="7925d-132">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="7925d-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="7925d-133">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="7925d-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="7925d-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="7925d-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="7925d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-135">None</span></span>   |<span data-ttu-id="7925d-136">Interrompa a sincronização e exclua permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="7925d-137">Obter synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="7925d-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="7925d-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="7925d-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="7925d-139">Recupere o esquema de sincronização efetiva do trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="7925d-140">Atualizar synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="7925d-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="7925d-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-141">None</span></span>   |<span data-ttu-id="7925d-142">Atualize o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="7925d-143">Validar credenciais</span><span class="sxs-lookup"><span data-stu-id="7925d-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="7925d-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7925d-144">None</span></span>|<span data-ttu-id="7925d-145">Teste as credenciais fornecidas em relação ao diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="7925d-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="7925d-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7925d-146">Properties</span></span>

| <span data-ttu-id="7925d-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7925d-147">Property</span></span>      | <span data-ttu-id="7925d-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="7925d-148">Type</span></span>      | <span data-ttu-id="7925d-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="7925d-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="7925d-150">id</span><span class="sxs-lookup"><span data-stu-id="7925d-150">id</span></span>             |<span data-ttu-id="7925d-151">String</span><span class="sxs-lookup"><span data-stu-id="7925d-151">String</span></span>                     |<span data-ttu-id="7925d-152">Identificador exclusivo do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7925d-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="7925d-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7925d-153">Read-only.</span></span>|
|<span data-ttu-id="7925d-154">futebol</span><span class="sxs-lookup"><span data-stu-id="7925d-154">schedule</span></span>       |[<span data-ttu-id="7925d-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="7925d-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="7925d-156">Agendamento usado para executar o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-156">Schedule used to run the job.</span></span> <span data-ttu-id="7925d-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7925d-157">Read-only.</span></span>|
|<span data-ttu-id="7925d-158">status</span><span class="sxs-lookup"><span data-stu-id="7925d-158">status</span></span>         |[<span data-ttu-id="7925d-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="7925d-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="7925d-160">Status do trabalho, que inclui quando o trabalho foi executado pela última vez, o estado atual do trabalho e os erros.</span><span class="sxs-lookup"><span data-stu-id="7925d-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="7925d-161">templateId</span><span class="sxs-lookup"><span data-stu-id="7925d-161">templateId</span></span>     |<span data-ttu-id="7925d-162">String</span><span class="sxs-lookup"><span data-stu-id="7925d-162">String</span></span>    |<span data-ttu-id="7925d-163">Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que este trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="7925d-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7925d-164">Relações</span><span class="sxs-lookup"><span data-stu-id="7925d-164">Relationships</span></span>
| <span data-ttu-id="7925d-165">Relação</span><span class="sxs-lookup"><span data-stu-id="7925d-165">Relationship</span></span> | <span data-ttu-id="7925d-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="7925d-166">Type</span></span>   |<span data-ttu-id="7925d-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="7925d-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7925d-168">esquemas</span><span class="sxs-lookup"><span data-stu-id="7925d-168">schema</span></span>|[<span data-ttu-id="7925d-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="7925d-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="7925d-170">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7925d-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7925d-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7925d-171">JSON representation</span></span>

<span data-ttu-id="7925d-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7925d-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
