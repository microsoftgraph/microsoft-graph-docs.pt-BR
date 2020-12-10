---
title: tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5833dc1f37620a419153100ebf9ce6d7f141fa5d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617007"
---
# <a name="printer-resource-type"></a><span data-ttu-id="40b62-104">tipo de recurso de impressora</span><span class="sxs-lookup"><span data-stu-id="40b62-104">printer resource type</span></span>

<span data-ttu-id="40b62-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40b62-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b62-106">Representa um dispositivo de impressora que foi registrado com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="40b62-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="40b62-107">Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.</span><span class="sxs-lookup"><span data-stu-id="40b62-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="40b62-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="40b62-108">Methods</span></span>

| <span data-ttu-id="40b62-109">Método</span><span class="sxs-lookup"><span data-stu-id="40b62-109">Method</span></span>       | <span data-ttu-id="40b62-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40b62-110">Return Type</span></span> | <span data-ttu-id="40b62-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b62-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="40b62-112">Criar</span><span class="sxs-lookup"><span data-stu-id="40b62-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="40b62-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="40b62-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="40b62-114">Criar (registrar) uma nova impressora com impressão universal.</span><span class="sxs-lookup"><span data-stu-id="40b62-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="40b62-115">Get</span><span class="sxs-lookup"><span data-stu-id="40b62-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="40b62-116">impressora</span><span class="sxs-lookup"><span data-stu-id="40b62-116">printer</span></span>](printer.md) | <span data-ttu-id="40b62-117">Leia as propriedades e as relações do objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="40b62-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="40b62-118">Update</span><span class="sxs-lookup"><span data-stu-id="40b62-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="40b62-119">impressora</span><span class="sxs-lookup"><span data-stu-id="40b62-119">printer</span></span>](printer.md) | <span data-ttu-id="40b62-120">Atualize o objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="40b62-120">Update the printer object.</span></span> |
| [<span data-ttu-id="40b62-121">Delete</span><span class="sxs-lookup"><span data-stu-id="40b62-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="40b62-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b62-122">None</span></span> | <span data-ttu-id="40b62-123">Cancelar o registro da impressora física do serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="40b62-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="40b62-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="40b62-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="40b62-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b62-125">None</span></span> | <span data-ttu-id="40b62-126">Restaurar as configurações padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="40b62-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="40b62-127">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="40b62-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="40b62-128">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="40b62-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="40b62-129">Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="40b62-130">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="40b62-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="40b62-131">Impressão</span><span class="sxs-lookup"><span data-stu-id="40b62-131">printJob</span></span>](printjob.md) | <span data-ttu-id="40b62-132">Crie um novo trabalho de impressão para a impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-132">Create a new print job for the printer.</span></span> <span data-ttu-id="40b62-133">Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="40b62-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="40b62-134">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="40b62-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="40b62-135">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="40b62-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="40b62-136">Obter uma lista de conectores aos quais esta impressora está associada.</span><span class="sxs-lookup"><span data-stu-id="40b62-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="40b62-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="40b62-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="40b62-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b62-138">None</span></span> | <span data-ttu-id="40b62-139">Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="40b62-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="40b62-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="40b62-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="40b62-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="40b62-142">Crie um [printTaskTrigger](printtasktrigger.md) que seja executado quando os eventos Print ocorrerem.</span><span class="sxs-lookup"><span data-stu-id="40b62-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="40b62-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="40b62-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="40b62-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b62-144">None</span></span> | <span data-ttu-id="40b62-145">Excluir um [printTaskTrigger](printtasktrigger.md) que está associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="40b62-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b62-146">Properties</span></span>
| <span data-ttu-id="40b62-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b62-147">Property</span></span>     | <span data-ttu-id="40b62-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b62-148">Type</span></span>        | <span data-ttu-id="40b62-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b62-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40b62-150">id</span><span class="sxs-lookup"><span data-stu-id="40b62-150">id</span></span>|<span data-ttu-id="40b62-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40b62-151">String</span></span>|<span data-ttu-id="40b62-152">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="40b62-152">The document's identifier.</span></span> <span data-ttu-id="40b62-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b62-153">Read-only.</span></span>|
|<span data-ttu-id="40b62-154">displayName</span><span class="sxs-lookup"><span data-stu-id="40b62-154">displayName</span></span>|<span data-ttu-id="40b62-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40b62-155">String</span></span>|<span data-ttu-id="40b62-156">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-156">The name of the printer.</span></span>|
|<span data-ttu-id="40b62-157">fabricante</span><span class="sxs-lookup"><span data-stu-id="40b62-157">manufacturer</span></span>|<span data-ttu-id="40b62-158">String</span><span class="sxs-lookup"><span data-stu-id="40b62-158">String</span></span>|<span data-ttu-id="40b62-159">O fabricante relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-159">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="40b62-160">modelo</span><span class="sxs-lookup"><span data-stu-id="40b62-160">model</span></span>|<span data-ttu-id="40b62-161">String</span><span class="sxs-lookup"><span data-stu-id="40b62-161">String</span></span>|<span data-ttu-id="40b62-162">O nome do modelo relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-162">The model name reported by the printer.</span></span>|
|<span data-ttu-id="40b62-163">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="40b62-163">registeredDateTime</span></span>|<span data-ttu-id="40b62-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40b62-164">DateTimeOffset</span></span>|<span data-ttu-id="40b62-165">O DateTimeOffset quando a impressora foi registrada.</span><span class="sxs-lookup"><span data-stu-id="40b62-165">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="40b62-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b62-166">Read-only.</span></span>|
|<span data-ttu-id="40b62-167">status</span><span class="sxs-lookup"><span data-stu-id="40b62-167">status</span></span>|[<span data-ttu-id="40b62-168">printerStatus</span><span class="sxs-lookup"><span data-stu-id="40b62-168">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="40b62-169">O status de processamento da impressora, incluindo erros.</span><span class="sxs-lookup"><span data-stu-id="40b62-169">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="40b62-170">isShared</span><span class="sxs-lookup"><span data-stu-id="40b62-170">isShared</span></span>|<span data-ttu-id="40b62-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="40b62-171">Boolean</span></span>|<span data-ttu-id="40b62-172">True se a impressora é compartilhada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="40b62-172">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="40b62-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b62-173">Read-only.</span></span>|
|<span data-ttu-id="40b62-174">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="40b62-174">hasPhysicalDevice</span></span>|<span data-ttu-id="40b62-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="40b62-175">Boolean</span></span>|<span data-ttu-id="40b62-176">True se a impressora tem um dispositivo físico para impressão.</span><span class="sxs-lookup"><span data-stu-id="40b62-176">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="40b62-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b62-177">Read-only.</span></span>|
|<span data-ttu-id="40b62-178">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="40b62-178">isAcceptingJobs</span></span>|<span data-ttu-id="40b62-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="40b62-179">Boolean</span></span>|<span data-ttu-id="40b62-180">Se a impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="40b62-180">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="40b62-181">location</span><span class="sxs-lookup"><span data-stu-id="40b62-181">location</span></span>|[<span data-ttu-id="40b62-182">printerLocation</span><span class="sxs-lookup"><span data-stu-id="40b62-182">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="40b62-183">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-183">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="40b62-184">defaults</span><span class="sxs-lookup"><span data-stu-id="40b62-184">defaults</span></span>|[<span data-ttu-id="40b62-185">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="40b62-185">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="40b62-186">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-186">The printer's default print settings.</span></span>|
|<span data-ttu-id="40b62-187">capabilities</span><span class="sxs-lookup"><span data-stu-id="40b62-187">capabilities</span></span>|[<span data-ttu-id="40b62-188">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="40b62-188">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="40b62-189">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-189">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40b62-190">Relações</span><span class="sxs-lookup"><span data-stu-id="40b62-190">Relationships</span></span>
| <span data-ttu-id="40b62-191">Relação</span><span class="sxs-lookup"><span data-stu-id="40b62-191">Relationship</span></span> | <span data-ttu-id="40b62-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b62-192">Type</span></span>        | <span data-ttu-id="40b62-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b62-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40b62-194">jobs</span><span class="sxs-lookup"><span data-stu-id="40b62-194">jobs</span></span>|<span data-ttu-id="40b62-195">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="40b62-195">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="40b62-196">A lista de trabalhos que estão na fila para impressão pela impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-196">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="40b62-197">shares</span><span class="sxs-lookup"><span data-stu-id="40b62-197">shares</span></span>|<span data-ttu-id="40b62-198">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="40b62-198">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="40b62-199">A lista de printerShares que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-199">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="40b62-200">Atualmente, apenas um printerShare pode ser associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-200">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="40b62-201">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b62-201">Read-only.</span></span> <span data-ttu-id="40b62-202">Anulável.</span><span class="sxs-lookup"><span data-stu-id="40b62-202">Nullable.</span></span>|
|<span data-ttu-id="40b62-203">conectores</span><span class="sxs-lookup"><span data-stu-id="40b62-203">connectors</span></span>|[<span data-ttu-id="40b62-204">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="40b62-204">printConnector</span></span>](printconnector.md)|<span data-ttu-id="40b62-205">Os conectores associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-205">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="40b62-206">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="40b62-206">taskTriggers</span></span>|<span data-ttu-id="40b62-207">coleção [printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="40b62-207">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="40b62-208">Uma lista de disparadores de tarefas que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="40b62-208">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b62-209">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b62-209">JSON representation</span></span>

<span data-ttu-id="40b62-210">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40b62-210">The following is a JSON representation of the resource.</span></span>

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


