---
title: tipo de recurso de synchronizationJob
description: Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente. O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário. Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.
localization_priority: Normal
ms.openlocfilehash: 4d65f39cd63357c8fc7c1e22d3d3871eb1646d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892145"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="1f1b7-105">tipo de recurso de synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1f1b7-105">synchronizationJob resource type</span></span>

> <span data-ttu-id="1f1b7-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f1b7-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f1b7-108">Executa a sincronização por executar periodicamente em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-108">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="1f1b7-109">O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-109">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="1f1b7-110">Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-110">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="1f1b7-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="1f1b7-111">Methods</span></span>

| <span data-ttu-id="1f1b7-112">Método</span><span class="sxs-lookup"><span data-stu-id="1f1b7-112">Method</span></span>        | <span data-ttu-id="1f1b7-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1f1b7-113">Return Type</span></span>               | <span data-ttu-id="1f1b7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f1b7-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="1f1b7-115">List</span><span class="sxs-lookup"><span data-stu-id="1f1b7-115">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="1f1b7-116">coleção [synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="1f1b7-116">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="1f1b7-117">Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="1f1b7-117">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="1f1b7-118">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1f1b7-118">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="1f1b7-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1f1b7-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="1f1b7-120">Leia as propriedades e os relacionamentos de um objeto synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-120">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="1f1b7-121">Create</span><span class="sxs-lookup"><span data-stu-id="1f1b7-121">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="1f1b7-122">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1f1b7-122">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="1f1b7-123">Crie um novo trabalho para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-123">Create new job for a given application.</span></span>|
|[<span data-ttu-id="1f1b7-124">Start</span><span class="sxs-lookup"><span data-stu-id="1f1b7-124">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="1f1b7-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-125">None</span></span>   |<span data-ttu-id="1f1b7-126">Inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-126">Start synchronization.</span></span> <span data-ttu-id="1f1b7-127">Se o trabalho estiver em um estado pausado, ele continua do ponto onde o trabalho foi pausado.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-127">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="1f1b7-128">Se o trabalho estiver em quarentena, o status de quarentena está desmarcado.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-128">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="1f1b7-129">Restart</span><span class="sxs-lookup"><span data-stu-id="1f1b7-129">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="1f1b7-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-130">None</span></span>   |<span data-ttu-id="1f1b7-131">Força o trabalho recomece e processar novamente todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-131">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="1f1b7-132">Pause</span><span class="sxs-lookup"><span data-stu-id="1f1b7-132">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="1f1b7-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-133">None</span></span>   |<span data-ttu-id="1f1b7-134">Interrompa temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-134">Temporarily stop synchronization.</span></span> <span data-ttu-id="1f1b7-135">Todos o andamento, incluindo o estado do trabalho é persistente e o trabalho continuará de onde ela parou quando uma chamada [Iniciar](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-135">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="1f1b7-136">Delete</span><span class="sxs-lookup"><span data-stu-id="1f1b7-136">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="1f1b7-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-137">None</span></span>   |<span data-ttu-id="1f1b7-138">Parar de sincronização e excluir permanentemente todo o estado associado ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-138">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="1f1b7-139">Obter synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="1f1b7-139">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="1f1b7-140">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1f1b7-140">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="1f1b7-141">Recupere o esquema de sincronização efetivo do trabalho.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-141">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="1f1b7-142">Atualizar synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="1f1b7-142">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="1f1b7-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-143">None</span></span>   |<span data-ttu-id="1f1b7-144">Atualize esquema de sincronização de tarefa.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-144">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="1f1b7-145">Validar as credenciais</span><span class="sxs-lookup"><span data-stu-id="1f1b7-145">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="1f1b7-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1b7-146">None</span></span>|<span data-ttu-id="1f1b7-147">Teste as credenciais fornecidas com o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-147">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f1b7-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f1b7-148">Properties</span></span>

| <span data-ttu-id="1f1b7-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f1b7-149">Property</span></span>      | <span data-ttu-id="1f1b7-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f1b7-150">Type</span></span>      | <span data-ttu-id="1f1b7-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f1b7-151">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1f1b7-152">id</span><span class="sxs-lookup"><span data-stu-id="1f1b7-152">id</span></span>             |<span data-ttu-id="1f1b7-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f1b7-153">String</span></span>                     |<span data-ttu-id="1f1b7-154">Identificador de trabalho de sincronização exclusivo.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-154">Unique synchronization job identifier.</span></span> <span data-ttu-id="1f1b7-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-155">Read-only.</span></span>|
|<span data-ttu-id="1f1b7-156">agenda</span><span class="sxs-lookup"><span data-stu-id="1f1b7-156">schedule</span></span>       |[<span data-ttu-id="1f1b7-157">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="1f1b7-157">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="1f1b7-158">Usada para executar o trabalho de agendamento.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-158">Schedule used to run the job.</span></span> <span data-ttu-id="1f1b7-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-159">Read-only.</span></span>|
|<span data-ttu-id="1f1b7-160">status</span><span class="sxs-lookup"><span data-stu-id="1f1b7-160">status</span></span>         |[<span data-ttu-id="1f1b7-161">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="1f1b7-161">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="1f1b7-162">Status do trabalho, que inclui quando o trabalho foi executado último, o estado atual do trabalho e erros.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-162">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="1f1b7-163">templateId</span><span class="sxs-lookup"><span data-stu-id="1f1b7-163">templateId</span></span>     |<span data-ttu-id="1f1b7-164">String</span><span class="sxs-lookup"><span data-stu-id="1f1b7-164">String</span></span>    |<span data-ttu-id="1f1b7-165">Identificador do [modelo de sincronização](synchronization-synchronizationtemplate.md) em que esse trabalho se baseia.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-165">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f1b7-166">Relações</span><span class="sxs-lookup"><span data-stu-id="1f1b7-166">Relationships</span></span>
| <span data-ttu-id="1f1b7-167">Relação</span><span class="sxs-lookup"><span data-stu-id="1f1b7-167">Relationship</span></span> | <span data-ttu-id="1f1b7-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f1b7-168">Type</span></span>   |<span data-ttu-id="1f1b7-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f1b7-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f1b7-170">esquema</span><span class="sxs-lookup"><span data-stu-id="1f1b7-170">schema</span></span>|[<span data-ttu-id="1f1b7-171">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1f1b7-171">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="1f1b7-172">O esquema de sincronização configurado para o trabalho.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-172">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f1b7-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f1b7-173">JSON representation</span></span>

<span data-ttu-id="1f1b7-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f1b7-174">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
