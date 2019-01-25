---
title: tipo de recurso de synchronizationJob
description: Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente. O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário. Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510565"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="94f4b-105">tipo de recurso de synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="94f4b-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94f4b-106">Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente.</span><span class="sxs-lookup"><span data-stu-id="94f4b-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="94f4b-107">O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário.</span><span class="sxs-lookup"><span data-stu-id="94f4b-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="94f4b-108">Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.</span><span class="sxs-lookup"><span data-stu-id="94f4b-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="94f4b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="94f4b-109">Methods</span></span>

| <span data-ttu-id="94f4b-110">Método</span><span class="sxs-lookup"><span data-stu-id="94f4b-110">Method</span></span>        | <span data-ttu-id="94f4b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="94f4b-111">Return Type</span></span>               | <span data-ttu-id="94f4b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f4b-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="94f4b-113">List</span><span class="sxs-lookup"><span data-stu-id="94f4b-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="94f4b-114">coleção [synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="94f4b-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="94f4b-115">Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="94f4b-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="94f4b-116">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="94f4b-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="94f4b-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="94f4b-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="94f4b-118">Leia as propriedades e os relacionamentos de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="94f4b-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="94f4b-119">Create</span><span class="sxs-lookup"><span data-stu-id="94f4b-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="94f4b-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="94f4b-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="94f4b-121">Crie um novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="94f4b-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="94f4b-122">Start</span><span class="sxs-lookup"><span data-stu-id="94f4b-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="94f4b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-123">None</span></span>   |<span data-ttu-id="94f4b-124">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="94f4b-124">Start synchronization.</span></span> <span data-ttu-id="94f4b-125">Se o trabalho estiver em um estado pausado, ele continua do ponto onde o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="94f4b-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="94f4b-126">Se o trabalho estiver em quarentena, o status de quarentena está desmarcado.</span><span class="sxs-lookup"><span data-stu-id="94f4b-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="94f4b-127">Restart</span><span class="sxs-lookup"><span data-stu-id="94f4b-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="94f4b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-128">None</span></span>   |<span data-ttu-id="94f4b-129">Força o trabalho recomece e processar novamente todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="94f4b-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="94f4b-130">Pause</span><span class="sxs-lookup"><span data-stu-id="94f4b-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="94f4b-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-131">None</span></span>   |<span data-ttu-id="94f4b-132">Interrompa temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="94f4b-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="94f4b-133">Todos o andamento, incluindo o estado do trabalho é persistente e o trabalho continuará de onde ela parou quando uma chamada [Iniciar](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="94f4b-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="94f4b-134">Delete</span><span class="sxs-lookup"><span data-stu-id="94f4b-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="94f4b-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-135">None</span></span>   |<span data-ttu-id="94f4b-136">Parar de sincronização e excluir permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="94f4b-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="94f4b-137">Obter synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="94f4b-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="94f4b-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="94f4b-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="94f4b-139">Recupere o esquema de sincronização efetivo do trabalho.</span><span class="sxs-lookup"><span data-stu-id="94f4b-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="94f4b-140">Atualizar synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="94f4b-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="94f4b-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-141">None</span></span>   |<span data-ttu-id="94f4b-142">Atualize esquema de sincronização de tarefa.</span><span class="sxs-lookup"><span data-stu-id="94f4b-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="94f4b-143">Validar as credenciais</span><span class="sxs-lookup"><span data-stu-id="94f4b-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="94f4b-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94f4b-144">None</span></span>|<span data-ttu-id="94f4b-145">Teste as credenciais fornecidas com o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="94f4b-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="94f4b-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94f4b-146">Properties</span></span>

| <span data-ttu-id="94f4b-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94f4b-147">Property</span></span>      | <span data-ttu-id="94f4b-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="94f4b-148">Type</span></span>      | <span data-ttu-id="94f4b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f4b-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="94f4b-150">id</span><span class="sxs-lookup"><span data-stu-id="94f4b-150">id</span></span>             |<span data-ttu-id="94f4b-151">String</span><span class="sxs-lookup"><span data-stu-id="94f4b-151">String</span></span>                     |<span data-ttu-id="94f4b-152">Identificador de trabalho de sincronização exclusivo.</span><span class="sxs-lookup"><span data-stu-id="94f4b-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="94f4b-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94f4b-153">Read-only.</span></span>|
|<span data-ttu-id="94f4b-154">Schedule</span><span class="sxs-lookup"><span data-stu-id="94f4b-154">schedule</span></span>       |[<span data-ttu-id="94f4b-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="94f4b-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="94f4b-156">Usada para executar o trabalho de agendamento.</span><span class="sxs-lookup"><span data-stu-id="94f4b-156">Schedule used to run the job.</span></span> <span data-ttu-id="94f4b-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94f4b-157">Read-only.</span></span>|
|<span data-ttu-id="94f4b-158">status</span><span class="sxs-lookup"><span data-stu-id="94f4b-158">status</span></span>         |[<span data-ttu-id="94f4b-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="94f4b-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="94f4b-160">Status do trabalho, que inclui quando o trabalho foi executado último, o estado atual do trabalho e erros.</span><span class="sxs-lookup"><span data-stu-id="94f4b-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="94f4b-161">templateId</span><span class="sxs-lookup"><span data-stu-id="94f4b-161">templateId</span></span>     |<span data-ttu-id="94f4b-162">String</span><span class="sxs-lookup"><span data-stu-id="94f4b-162">String</span></span>    |<span data-ttu-id="94f4b-163">Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que esse trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="94f4b-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94f4b-164">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="94f4b-164">Relationships</span></span>
| <span data-ttu-id="94f4b-165">Relação</span><span class="sxs-lookup"><span data-stu-id="94f4b-165">Relationship</span></span> | <span data-ttu-id="94f4b-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="94f4b-166">Type</span></span>   |<span data-ttu-id="94f4b-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f4b-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94f4b-168">SCHEMA</span><span class="sxs-lookup"><span data-stu-id="94f4b-168">schema</span></span>|[<span data-ttu-id="94f4b-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="94f4b-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="94f4b-170">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="94f4b-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94f4b-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94f4b-171">JSON representation</span></span>

<span data-ttu-id="94f4b-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94f4b-172">The following is a JSON representation of the resource.</span></span>

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
