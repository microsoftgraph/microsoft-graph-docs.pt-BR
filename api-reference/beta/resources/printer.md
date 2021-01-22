---
title: tipo de recurso printer
description: Representa um dispositivo de impressora física que foi registrado com o serviço de Impressão Universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934867"
---
# <a name="printer-resource-type"></a><span data-ttu-id="97dea-104">tipo de recurso printer</span><span class="sxs-lookup"><span data-stu-id="97dea-104">printer resource type</span></span>

<span data-ttu-id="97dea-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97dea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97dea-106">Representa um dispositivo de impressora que foi registrado com o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="97dea-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="97dea-107">Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.</span><span class="sxs-lookup"><span data-stu-id="97dea-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="97dea-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="97dea-108">This resource supports:</span></span>
* <span data-ttu-id="97dea-109">[Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).</span><span class="sxs-lookup"><span data-stu-id="97dea-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="97dea-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="97dea-110">Methods</span></span>

| <span data-ttu-id="97dea-111">Método</span><span class="sxs-lookup"><span data-stu-id="97dea-111">Method</span></span>       | <span data-ttu-id="97dea-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="97dea-112">Return Type</span></span> | <span data-ttu-id="97dea-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="97dea-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="97dea-114">Criar</span><span class="sxs-lookup"><span data-stu-id="97dea-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="97dea-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="97dea-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="97dea-116">Crie (registre) uma nova impressora com Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="97dea-116">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="97dea-117">Get</span><span class="sxs-lookup"><span data-stu-id="97dea-117">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="97dea-118">impressora</span><span class="sxs-lookup"><span data-stu-id="97dea-118">printer</span></span>](printer.md) | <span data-ttu-id="97dea-119">Leia as propriedades e os relacionamentos do objeto printer.</span><span class="sxs-lookup"><span data-stu-id="97dea-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="97dea-120">Update</span><span class="sxs-lookup"><span data-stu-id="97dea-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="97dea-121">impressora</span><span class="sxs-lookup"><span data-stu-id="97dea-121">printer</span></span>](printer.md) | <span data-ttu-id="97dea-122">Atualize o objeto printer.</span><span class="sxs-lookup"><span data-stu-id="97dea-122">Update the printer object.</span></span> |
| [<span data-ttu-id="97dea-123">Delete</span><span class="sxs-lookup"><span data-stu-id="97dea-123">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="97dea-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97dea-124">None</span></span> | <span data-ttu-id="97dea-125">Unregister the physical printer from the Universal Print service.</span><span class="sxs-lookup"><span data-stu-id="97dea-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="97dea-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="97dea-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="97dea-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97dea-127">None</span></span> | <span data-ttu-id="97dea-128">Restaure as configurações padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="97dea-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="97dea-129">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="97dea-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="97dea-130">[Coleção printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="97dea-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="97dea-131">Obter uma lista de trabalhos de impressão que estão na fila para processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="97dea-132">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="97dea-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="97dea-133">printJob</span><span class="sxs-lookup"><span data-stu-id="97dea-133">printJob</span></span>](printjob.md) | <span data-ttu-id="97dea-134">Crie um novo trabalho de impressão para a impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-134">Create a new print job for the printer.</span></span> <span data-ttu-id="97dea-135">Para começar a imprimir o trabalho, use [start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="97dea-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="97dea-136">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="97dea-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="97dea-137">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="97dea-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="97dea-138">Obter uma lista de conectores aos que esta impressora está associada.</span><span class="sxs-lookup"><span data-stu-id="97dea-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="97dea-139">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="97dea-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="97dea-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97dea-140">None</span></span> | <span data-ttu-id="97dea-141">Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="97dea-142">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="97dea-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="97dea-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="97dea-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="97dea-144">Crie um [printTaskTrigger que](printtasktrigger.md) seja executado quando ocorrerem eventos de impressão.</span><span class="sxs-lookup"><span data-stu-id="97dea-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="97dea-145">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="97dea-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="97dea-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97dea-146">None</span></span> | <span data-ttu-id="97dea-147">[Exclua um printTaskTrigger](printtasktrigger.md) associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="97dea-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97dea-148">Properties</span></span>
| <span data-ttu-id="97dea-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97dea-149">Property</span></span>     | <span data-ttu-id="97dea-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="97dea-150">Type</span></span>        | <span data-ttu-id="97dea-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="97dea-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97dea-152">id</span><span class="sxs-lookup"><span data-stu-id="97dea-152">id</span></span>|<span data-ttu-id="97dea-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97dea-153">String</span></span>|<span data-ttu-id="97dea-154">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="97dea-154">The document's identifier.</span></span> <span data-ttu-id="97dea-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97dea-155">Read-only.</span></span>|
|<span data-ttu-id="97dea-156">displayName</span><span class="sxs-lookup"><span data-stu-id="97dea-156">displayName</span></span>|<span data-ttu-id="97dea-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97dea-157">String</span></span>|<span data-ttu-id="97dea-158">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-158">The name of the printer.</span></span>|
|<span data-ttu-id="97dea-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="97dea-159">manufacturer</span></span>|<span data-ttu-id="97dea-160">String</span><span class="sxs-lookup"><span data-stu-id="97dea-160">String</span></span>|<span data-ttu-id="97dea-161">O fabricante relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="97dea-162">modelo</span><span class="sxs-lookup"><span data-stu-id="97dea-162">model</span></span>|<span data-ttu-id="97dea-163">String</span><span class="sxs-lookup"><span data-stu-id="97dea-163">String</span></span>|<span data-ttu-id="97dea-164">O nome do modelo relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="97dea-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="97dea-165">registeredDateTime</span></span>|<span data-ttu-id="97dea-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97dea-166">DateTimeOffset</span></span>|<span data-ttu-id="97dea-167">DateTimeOffset quando a impressora foi registrada.</span><span class="sxs-lookup"><span data-stu-id="97dea-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="97dea-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97dea-168">Read-only.</span></span>|
|<span data-ttu-id="97dea-169">status</span><span class="sxs-lookup"><span data-stu-id="97dea-169">status</span></span>|[<span data-ttu-id="97dea-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="97dea-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="97dea-171">O status de processamento da impressora, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="97dea-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="97dea-172">isShared</span><span class="sxs-lookup"><span data-stu-id="97dea-172">isShared</span></span>|<span data-ttu-id="97dea-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="97dea-173">Boolean</span></span>|<span data-ttu-id="97dea-174">True se a impressora for compartilhada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="97dea-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="97dea-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97dea-175">Read-only.</span></span>|
|<span data-ttu-id="97dea-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="97dea-176">hasPhysicalDevice</span></span>|<span data-ttu-id="97dea-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="97dea-177">Boolean</span></span>|<span data-ttu-id="97dea-178">True se a impressora tiver um dispositivo físico para impressão.</span><span class="sxs-lookup"><span data-stu-id="97dea-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="97dea-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97dea-179">Read-only.</span></span>|
|<span data-ttu-id="97dea-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="97dea-180">isAcceptingJobs</span></span>|<span data-ttu-id="97dea-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="97dea-181">Boolean</span></span>|<span data-ttu-id="97dea-182">Se a impressora está aceitando novos trabalhos de impressão no momento.</span><span class="sxs-lookup"><span data-stu-id="97dea-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="97dea-183">location</span><span class="sxs-lookup"><span data-stu-id="97dea-183">location</span></span>|[<span data-ttu-id="97dea-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="97dea-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="97dea-185">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="97dea-186">defaults</span><span class="sxs-lookup"><span data-stu-id="97dea-186">defaults</span></span>|[<span data-ttu-id="97dea-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="97dea-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="97dea-188">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="97dea-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="97dea-189">capabilities</span></span>|[<span data-ttu-id="97dea-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="97dea-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="97dea-191">Os recursos da impressora associada a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-191">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97dea-192">Relações</span><span class="sxs-lookup"><span data-stu-id="97dea-192">Relationships</span></span>
| <span data-ttu-id="97dea-193">Relação</span><span class="sxs-lookup"><span data-stu-id="97dea-193">Relationship</span></span> | <span data-ttu-id="97dea-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="97dea-194">Type</span></span>        | <span data-ttu-id="97dea-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="97dea-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97dea-196">jobs</span><span class="sxs-lookup"><span data-stu-id="97dea-196">jobs</span></span>|<span data-ttu-id="97dea-197">[Coleção printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="97dea-197">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="97dea-198">A lista de trabalhos que estão na fila para impressão pela impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-198">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="97dea-199">shares</span><span class="sxs-lookup"><span data-stu-id="97dea-199">shares</span></span>|<span data-ttu-id="97dea-200">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="97dea-200">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="97dea-201">A lista de printerShares que estão associadas à impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-201">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="97dea-202">Atualmente, apenas uma printerShare pode ser associada à impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-202">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="97dea-203">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97dea-203">Read-only.</span></span> <span data-ttu-id="97dea-204">Anulável.</span><span class="sxs-lookup"><span data-stu-id="97dea-204">Nullable.</span></span>|
|<span data-ttu-id="97dea-205">conectores</span><span class="sxs-lookup"><span data-stu-id="97dea-205">connectors</span></span>|[<span data-ttu-id="97dea-206">printConnector</span><span class="sxs-lookup"><span data-stu-id="97dea-206">printConnector</span></span>](printconnector.md)|<span data-ttu-id="97dea-207">Os conectores associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-207">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="97dea-208">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="97dea-208">taskTriggers</span></span>|<span data-ttu-id="97dea-209">[Coleção printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="97dea-209">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="97dea-210">Uma lista de gatilhos de tarefa que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="97dea-210">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97dea-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97dea-211">JSON representation</span></span>

<span data-ttu-id="97dea-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97dea-212">The following is a JSON representation of the resource.</span></span>

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


