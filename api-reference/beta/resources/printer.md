---
title: Tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d90bf05b77c8843fc9fa5e5f32ecae29ffdaf48e
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765913"
---
# <a name="printer-resource-type"></a><span data-ttu-id="bb4b4-104">Tipo de recurso de impressora</span><span class="sxs-lookup"><span data-stu-id="bb4b4-104">printer resource type</span></span>

<span data-ttu-id="bb4b4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4b4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb4b4-106">Representa um dispositivo de impressora que foi registrado com o serviço impressão universal.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="bb4b4-107">Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="bb4b4-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="bb4b4-108">This resource supports:</span></span>
* <span data-ttu-id="bb4b4-109">[Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).</span><span class="sxs-lookup"><span data-stu-id="bb4b4-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="bb4b4-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="bb4b4-110">Methods</span></span>

| <span data-ttu-id="bb4b4-111">Método</span><span class="sxs-lookup"><span data-stu-id="bb4b4-111">Method</span></span>       | <span data-ttu-id="bb4b4-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb4b4-112">Return Type</span></span> | <span data-ttu-id="bb4b4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4b4-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bb4b4-114">Criar</span><span class="sxs-lookup"><span data-stu-id="bb4b4-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="bb4b4-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="bb4b4-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="bb4b4-116">Criar (registrar) uma nova impressora com Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-116">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="bb4b4-117">Get</span><span class="sxs-lookup"><span data-stu-id="bb4b4-117">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="bb4b4-118">impressora</span><span class="sxs-lookup"><span data-stu-id="bb4b4-118">printer</span></span>](printer.md) | <span data-ttu-id="bb4b4-119">Leia as propriedades e as relações do objeto printer.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="bb4b4-120">Atualizar</span><span class="sxs-lookup"><span data-stu-id="bb4b4-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="bb4b4-121">impressora</span><span class="sxs-lookup"><span data-stu-id="bb4b4-121">printer</span></span>](printer.md) | <span data-ttu-id="bb4b4-122">Atualize o objeto printer.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-122">Update the printer object.</span></span> |
| [<span data-ttu-id="bb4b4-123">Delete</span><span class="sxs-lookup"><span data-stu-id="bb4b4-123">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="bb4b4-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb4b4-124">None</span></span> | <span data-ttu-id="bb4b4-125">Desaconselhe a impressora física do serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="bb4b4-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="bb4b4-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="bb4b4-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb4b4-127">None</span></span> | <span data-ttu-id="bb4b4-128">Restaure as configurações padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="bb4b4-129">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="bb4b4-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="bb4b4-130">[Coleção printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b4-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="bb4b4-131">Obter uma lista de trabalhos de impressão que estão na fila para processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="bb4b4-132">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="bb4b4-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="bb4b4-133">printJob</span><span class="sxs-lookup"><span data-stu-id="bb4b4-133">printJob</span></span>](printjob.md) | <span data-ttu-id="bb4b4-134">Crie um novo trabalho de impressão para a impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-134">Create a new print job for the printer.</span></span> <span data-ttu-id="bb4b4-135">Para começar a imprimir o trabalho, use [start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b4-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="bb4b4-136">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="bb4b4-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="bb4b4-137">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b4-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="bb4b4-138">Obter uma lista de conectores que esta impressora está associada.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="bb4b4-139">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="bb4b4-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="bb4b4-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb4b4-140">None</span></span> | <span data-ttu-id="bb4b4-141">Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="bb4b4-142">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="bb4b4-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="bb4b4-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="bb4b4-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="bb4b4-144">Crie um [printTaskTrigger que](printtasktrigger.md) é executado quando ocorrem eventos de impressão.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="bb4b4-145">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="bb4b4-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="bb4b4-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb4b4-146">None</span></span> | <span data-ttu-id="bb4b4-147">[Exclua um printTaskTrigger](printtasktrigger.md) associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb4b4-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb4b4-148">Properties</span></span>
| <span data-ttu-id="bb4b4-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb4b4-149">Property</span></span>     | <span data-ttu-id="bb4b4-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4b4-150">Type</span></span>        | <span data-ttu-id="bb4b4-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4b4-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb4b4-152">id</span><span class="sxs-lookup"><span data-stu-id="bb4b4-152">id</span></span>|<span data-ttu-id="bb4b4-153">String</span><span class="sxs-lookup"><span data-stu-id="bb4b4-153">String</span></span>|<span data-ttu-id="bb4b4-154">O identificador da impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-154">The printer's identifier.</span></span> <span data-ttu-id="bb4b4-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-155">Read-only.</span></span>|
|<span data-ttu-id="bb4b4-156">displayName</span><span class="sxs-lookup"><span data-stu-id="bb4b4-156">displayName</span></span>|<span data-ttu-id="bb4b4-157">String</span><span class="sxs-lookup"><span data-stu-id="bb4b4-157">String</span></span>|<span data-ttu-id="bb4b4-158">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-158">The name of the printer.</span></span>|
|<span data-ttu-id="bb4b4-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="bb4b4-159">manufacturer</span></span>|<span data-ttu-id="bb4b4-160">String</span><span class="sxs-lookup"><span data-stu-id="bb4b4-160">String</span></span>|<span data-ttu-id="bb4b4-161">O fabricante relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="bb4b4-162">modelo</span><span class="sxs-lookup"><span data-stu-id="bb4b4-162">model</span></span>|<span data-ttu-id="bb4b4-163">String</span><span class="sxs-lookup"><span data-stu-id="bb4b4-163">String</span></span>|<span data-ttu-id="bb4b4-164">O nome do modelo relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="bb4b4-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="bb4b4-165">registeredDateTime</span></span>|<span data-ttu-id="bb4b4-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb4b4-166">DateTimeOffset</span></span>|<span data-ttu-id="bb4b4-167">DateTimeOffset quando a impressora foi registrada.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="bb4b4-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-168">Read-only.</span></span>|
|<span data-ttu-id="bb4b4-169">status</span><span class="sxs-lookup"><span data-stu-id="bb4b4-169">status</span></span>|[<span data-ttu-id="bb4b4-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="bb4b4-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="bb4b4-171">O status de processamento da impressora, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="bb4b4-172">isShared</span><span class="sxs-lookup"><span data-stu-id="bb4b4-172">isShared</span></span>|<span data-ttu-id="bb4b4-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4b4-173">Boolean</span></span>|<span data-ttu-id="bb4b4-174">True se a impressora for compartilhada; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="bb4b4-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-175">Read-only.</span></span>|
|<span data-ttu-id="bb4b4-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="bb4b4-176">hasPhysicalDevice</span></span>|<span data-ttu-id="bb4b4-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4b4-177">Boolean</span></span>|<span data-ttu-id="bb4b4-178">True se a impressora tiver um dispositivo físico para impressão.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="bb4b4-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-179">Read-only.</span></span>|
|<span data-ttu-id="bb4b4-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="bb4b4-180">isAcceptingJobs</span></span>|<span data-ttu-id="bb4b4-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4b4-181">Boolean</span></span>|<span data-ttu-id="bb4b4-182">Se a impressora está aceitando novos trabalhos de impressão no momento.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="bb4b4-183">localização</span><span class="sxs-lookup"><span data-stu-id="bb4b4-183">location</span></span>|[<span data-ttu-id="bb4b4-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="bb4b4-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="bb4b4-185">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="bb4b4-186">defaults</span><span class="sxs-lookup"><span data-stu-id="bb4b4-186">defaults</span></span>|[<span data-ttu-id="bb4b4-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="bb4b4-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="bb4b4-188">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="bb4b4-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="bb4b4-189">capabilities</span></span>|[<span data-ttu-id="bb4b4-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="bb4b4-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="bb4b4-191">Os recursos da impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-191">The capabilities of the printer.</span></span>|
|<span data-ttu-id="bb4b4-192">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="bb4b4-192">lastSeenDateTime</span></span>|<span data-ttu-id="bb4b4-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb4b4-193">DateTimeOffset</span></span>|<span data-ttu-id="bb4b4-194">O dateTimeOffset mais recente quando uma impressora interagiu com a Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-194">The most recent dateTimeOffset when a printer interacted with Universal Print.</span></span> <span data-ttu-id="bb4b4-195">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-195">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb4b4-196">Relações</span><span class="sxs-lookup"><span data-stu-id="bb4b4-196">Relationships</span></span>
| <span data-ttu-id="bb4b4-197">Relação</span><span class="sxs-lookup"><span data-stu-id="bb4b4-197">Relationship</span></span> | <span data-ttu-id="bb4b4-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4b4-198">Type</span></span>        | <span data-ttu-id="bb4b4-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4b4-199">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb4b4-200">jobs</span><span class="sxs-lookup"><span data-stu-id="bb4b4-200">jobs</span></span>|<span data-ttu-id="bb4b4-201">[Coleção printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b4-201">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="bb4b4-202">A lista de trabalhos que estão na fila para impressão pela impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-202">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="bb4b4-203">shares</span><span class="sxs-lookup"><span data-stu-id="bb4b4-203">shares</span></span>|<span data-ttu-id="bb4b4-204">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b4-204">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="bb4b4-205">A lista de printerShares que estão associadas à impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-205">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="bb4b4-206">Atualmente, apenas uma impressoraShare pode ser associada à impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-206">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="bb4b4-207">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-207">Read-only.</span></span> <span data-ttu-id="bb4b4-208">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-208">Nullable.</span></span>|
|<span data-ttu-id="bb4b4-209">conectores</span><span class="sxs-lookup"><span data-stu-id="bb4b4-209">connectors</span></span>|[<span data-ttu-id="bb4b4-210">printConnector</span><span class="sxs-lookup"><span data-stu-id="bb4b4-210">printConnector</span></span>](printconnector.md)|<span data-ttu-id="bb4b4-211">Os conectores associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-211">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="bb4b4-212">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="bb4b4-212">taskTriggers</span></span>|<span data-ttu-id="bb4b4-213">[Coleção printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b4-213">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="bb4b4-214">Uma lista de gatilhos de tarefas associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-214">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb4b4-215">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb4b4-215">JSON representation</span></span>

<span data-ttu-id="bb4b4-216">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb4b4-216">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "hasPhysicalDevice": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"},
  "lastSeenDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


