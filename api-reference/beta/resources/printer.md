---
title: tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2f1decf04f48f7ee8dc074997e6d503130bc74bc
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848616"
---
# <a name="printer-resource-type"></a><span data-ttu-id="1b98b-104">tipo de recurso de impressora</span><span class="sxs-lookup"><span data-stu-id="1b98b-104">printer resource type</span></span>

<span data-ttu-id="1b98b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b98b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b98b-106">Representa um dispositivo de impressora que foi registrado com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1b98b-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="1b98b-107">Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.</span><span class="sxs-lookup"><span data-stu-id="1b98b-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="1b98b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b98b-108">Methods</span></span>

| <span data-ttu-id="1b98b-109">Método</span><span class="sxs-lookup"><span data-stu-id="1b98b-109">Method</span></span>       | <span data-ttu-id="1b98b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b98b-110">Return Type</span></span> | <span data-ttu-id="1b98b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b98b-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b98b-112">Create</span><span class="sxs-lookup"><span data-stu-id="1b98b-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="1b98b-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="1b98b-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="1b98b-114">Criar (registrar) uma nova impressora com impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1b98b-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="1b98b-115">Get</span><span class="sxs-lookup"><span data-stu-id="1b98b-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="1b98b-116">impressora</span><span class="sxs-lookup"><span data-stu-id="1b98b-116">printer</span></span>](printer.md) | <span data-ttu-id="1b98b-117">Leia as propriedades e as relações do objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="1b98b-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="1b98b-118">Update</span><span class="sxs-lookup"><span data-stu-id="1b98b-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="1b98b-119">impressora</span><span class="sxs-lookup"><span data-stu-id="1b98b-119">printer</span></span>](printer.md) | <span data-ttu-id="1b98b-120">Atualize o objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="1b98b-120">Update the printer object.</span></span> |
| [<span data-ttu-id="1b98b-121">Delete</span><span class="sxs-lookup"><span data-stu-id="1b98b-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="1b98b-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b98b-122">None</span></span> | <span data-ttu-id="1b98b-123">Cancelar o registro da impressora física do serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1b98b-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="1b98b-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="1b98b-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="1b98b-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b98b-125">None</span></span> | <span data-ttu-id="1b98b-126">Restaurar as configurações padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="1b98b-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="1b98b-127">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="1b98b-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="1b98b-128">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1b98b-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="1b98b-129">Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="1b98b-130">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="1b98b-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="1b98b-131">Impressão</span><span class="sxs-lookup"><span data-stu-id="1b98b-131">printJob</span></span>](printjob.md) | <span data-ttu-id="1b98b-132">Crie um novo trabalho de impressão para a impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-132">Create a new print job for the printer.</span></span> <span data-ttu-id="1b98b-133">Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="1b98b-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="1b98b-134">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="1b98b-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="1b98b-135">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="1b98b-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="1b98b-136">Obter uma lista de conectores aos quais esta impressora está associada.</span><span class="sxs-lookup"><span data-stu-id="1b98b-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="1b98b-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="1b98b-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="1b98b-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b98b-138">None</span></span> | <span data-ttu-id="1b98b-139">Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="1b98b-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="1b98b-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="1b98b-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="1b98b-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="1b98b-142">Crie um [printTaskTrigger](printtasktrigger.md) que seja executado quando os eventos Print ocorrerem.</span><span class="sxs-lookup"><span data-stu-id="1b98b-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="1b98b-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="1b98b-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="1b98b-144">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b98b-144">None</span></span> | <span data-ttu-id="1b98b-145">Excluir um [printTaskTrigger](printtasktrigger.md) que está associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b98b-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b98b-146">Properties</span></span>
| <span data-ttu-id="1b98b-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b98b-147">Property</span></span>     | <span data-ttu-id="1b98b-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b98b-148">Type</span></span>        | <span data-ttu-id="1b98b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b98b-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b98b-150">id</span><span class="sxs-lookup"><span data-stu-id="1b98b-150">id</span></span>|<span data-ttu-id="1b98b-151">String</span><span class="sxs-lookup"><span data-stu-id="1b98b-151">String</span></span>|<span data-ttu-id="1b98b-152">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="1b98b-152">The document's identifier.</span></span> <span data-ttu-id="1b98b-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-153">Read-only.</span></span>|
|<span data-ttu-id="1b98b-154">displayName</span><span class="sxs-lookup"><span data-stu-id="1b98b-154">displayName</span></span>|<span data-ttu-id="1b98b-155">String</span><span class="sxs-lookup"><span data-stu-id="1b98b-155">String</span></span>|<span data-ttu-id="1b98b-156">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-156">The name of the printer.</span></span>|
|<span data-ttu-id="1b98b-157">fabricante</span><span class="sxs-lookup"><span data-stu-id="1b98b-157">manufacturer</span></span>|<span data-ttu-id="1b98b-158">String</span><span class="sxs-lookup"><span data-stu-id="1b98b-158">String</span></span>|<span data-ttu-id="1b98b-159">O fabricante relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-159">The manufacturer reported by the printer.</span></span> <span data-ttu-id="1b98b-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-160">Read-only.</span></span>|
|<span data-ttu-id="1b98b-161">modelo</span><span class="sxs-lookup"><span data-stu-id="1b98b-161">model</span></span>|<span data-ttu-id="1b98b-162">String</span><span class="sxs-lookup"><span data-stu-id="1b98b-162">String</span></span>|<span data-ttu-id="1b98b-163">O nome do modelo relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-163">The model name reported by the printer.</span></span> <span data-ttu-id="1b98b-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-164">Read-only.</span></span>|
|<span data-ttu-id="1b98b-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="1b98b-165">registeredDateTime</span></span>|<span data-ttu-id="1b98b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b98b-166">DateTimeOffset</span></span>|<span data-ttu-id="1b98b-167">O DateTimeOffset quando a impressora foi registrada.</span><span class="sxs-lookup"><span data-stu-id="1b98b-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="1b98b-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-168">Read-only.</span></span>|
|<span data-ttu-id="1b98b-169">status</span><span class="sxs-lookup"><span data-stu-id="1b98b-169">status</span></span>|[<span data-ttu-id="1b98b-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="1b98b-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="1b98b-171">O status de processamento da impressora, incluindo erros.</span><span class="sxs-lookup"><span data-stu-id="1b98b-171">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="1b98b-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-172">Read-only.</span></span>|
|<span data-ttu-id="1b98b-173">isShared</span><span class="sxs-lookup"><span data-stu-id="1b98b-173">isShared</span></span>|<span data-ttu-id="1b98b-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b98b-174">Boolean</span></span>|<span data-ttu-id="1b98b-175">True se a impressora é compartilhada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="1b98b-175">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="1b98b-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-176">Read-only.</span></span>|
|<span data-ttu-id="1b98b-177">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="1b98b-177">isAcceptingJobs</span></span>|<span data-ttu-id="1b98b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b98b-178">Boolean</span></span>|<span data-ttu-id="1b98b-179">Se a impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="1b98b-179">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="1b98b-180">location</span><span class="sxs-lookup"><span data-stu-id="1b98b-180">location</span></span>|[<span data-ttu-id="1b98b-181">printerLocation</span><span class="sxs-lookup"><span data-stu-id="1b98b-181">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="1b98b-182">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-182">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="1b98b-183">defaults</span><span class="sxs-lookup"><span data-stu-id="1b98b-183">defaults</span></span>|[<span data-ttu-id="1b98b-184">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="1b98b-184">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="1b98b-185">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-185">The printer's default print settings.</span></span>|
|<span data-ttu-id="1b98b-186">capabilities</span><span class="sxs-lookup"><span data-stu-id="1b98b-186">capabilities</span></span>|[<span data-ttu-id="1b98b-187">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="1b98b-187">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="1b98b-188">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-188">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b98b-189">Relações</span><span class="sxs-lookup"><span data-stu-id="1b98b-189">Relationships</span></span>
| <span data-ttu-id="1b98b-190">Relação</span><span class="sxs-lookup"><span data-stu-id="1b98b-190">Relationship</span></span> | <span data-ttu-id="1b98b-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b98b-191">Type</span></span>        | <span data-ttu-id="1b98b-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b98b-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b98b-193">jobs</span><span class="sxs-lookup"><span data-stu-id="1b98b-193">jobs</span></span>|<span data-ttu-id="1b98b-194">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1b98b-194">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="1b98b-195">A lista de trabalhos que estão na fila para impressão pela impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-195">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="1b98b-196">shares</span><span class="sxs-lookup"><span data-stu-id="1b98b-196">shares</span></span>|<span data-ttu-id="1b98b-197">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="1b98b-197">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="1b98b-198">A lista de printerShares que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-198">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="1b98b-199">Atualmente, apenas um printerShare pode ser associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-199">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="1b98b-200">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b98b-200">Read-only.</span></span> <span data-ttu-id="1b98b-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1b98b-201">Nullable.</span></span>|
|<span data-ttu-id="1b98b-202">conectores</span><span class="sxs-lookup"><span data-stu-id="1b98b-202">connectors</span></span>|[<span data-ttu-id="1b98b-203">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="1b98b-203">printConnector</span></span>](printconnector.md)|<span data-ttu-id="1b98b-204">Os conectores associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-204">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="1b98b-205">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="1b98b-205">taskTriggers</span></span>|<span data-ttu-id="1b98b-206">coleção [printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="1b98b-206">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="1b98b-207">Uma lista de disparadores de tarefas que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="1b98b-207">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b98b-208">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b98b-208">JSON representation</span></span>

<span data-ttu-id="1b98b-209">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b98b-209">The following is a JSON representation of the resource.</span></span>

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
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
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


