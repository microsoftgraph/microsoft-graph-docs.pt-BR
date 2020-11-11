---
title: tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 37c552a1239ee1d374c22be77ba81004cfc92e1f
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993952"
---
# <a name="printer-resource-type"></a><span data-ttu-id="b50e3-104">tipo de recurso de impressora</span><span class="sxs-lookup"><span data-stu-id="b50e3-104">printer resource type</span></span>

<span data-ttu-id="b50e3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b50e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b50e3-106">Representa um dispositivo de impressora que foi registrado com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="b50e3-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="b50e3-107">Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.</span><span class="sxs-lookup"><span data-stu-id="b50e3-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="b50e3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b50e3-108">Methods</span></span>

| <span data-ttu-id="b50e3-109">Método</span><span class="sxs-lookup"><span data-stu-id="b50e3-109">Method</span></span>       | <span data-ttu-id="b50e3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b50e3-110">Return Type</span></span> | <span data-ttu-id="b50e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b50e3-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b50e3-112">Create</span><span class="sxs-lookup"><span data-stu-id="b50e3-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="b50e3-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="b50e3-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="b50e3-114">Criar (registrar) uma nova impressora com impressão universal.</span><span class="sxs-lookup"><span data-stu-id="b50e3-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="b50e3-115">Get</span><span class="sxs-lookup"><span data-stu-id="b50e3-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="b50e3-116">impressora</span><span class="sxs-lookup"><span data-stu-id="b50e3-116">printer</span></span>](printer.md) | <span data-ttu-id="b50e3-117">Leia as propriedades e as relações do objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="b50e3-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="b50e3-118">Update</span><span class="sxs-lookup"><span data-stu-id="b50e3-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="b50e3-119">impressora</span><span class="sxs-lookup"><span data-stu-id="b50e3-119">printer</span></span>](printer.md) | <span data-ttu-id="b50e3-120">Atualize o objeto Printer.</span><span class="sxs-lookup"><span data-stu-id="b50e3-120">Update the printer object.</span></span> |
| [<span data-ttu-id="b50e3-121">Delete</span><span class="sxs-lookup"><span data-stu-id="b50e3-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="b50e3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b50e3-122">None</span></span> | <span data-ttu-id="b50e3-123">Cancelar o registro da impressora física do serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="b50e3-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="b50e3-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="b50e3-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="b50e3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b50e3-125">None</span></span> | <span data-ttu-id="b50e3-126">Restaurar as configurações padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="b50e3-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="b50e3-127">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="b50e3-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="b50e3-128">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b50e3-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="b50e3-129">Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pela impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="b50e3-130">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="b50e3-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="b50e3-131">Impressão</span><span class="sxs-lookup"><span data-stu-id="b50e3-131">printJob</span></span>](printjob.md) | <span data-ttu-id="b50e3-132">Crie um novo trabalho de impressão para a impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-132">Create a new print job for the printer.</span></span> <span data-ttu-id="b50e3-133">Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="b50e3-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="b50e3-134">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="b50e3-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="b50e3-135">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="b50e3-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="b50e3-136">Obter uma lista de conectores aos quais esta impressora está associada.</span><span class="sxs-lookup"><span data-stu-id="b50e3-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="b50e3-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="b50e3-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="b50e3-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b50e3-138">None</span></span> | <span data-ttu-id="b50e3-139">Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="b50e3-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b50e3-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="b50e3-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="b50e3-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="b50e3-142">Crie um [printTaskTrigger](printtasktrigger.md) que seja executado quando os eventos Print ocorrerem.</span><span class="sxs-lookup"><span data-stu-id="b50e3-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="b50e3-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b50e3-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="b50e3-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b50e3-144">None</span></span> | <span data-ttu-id="b50e3-145">Excluir um [printTaskTrigger](printtasktrigger.md) que está associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="b50e3-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b50e3-146">Properties</span></span>
| <span data-ttu-id="b50e3-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b50e3-147">Property</span></span>     | <span data-ttu-id="b50e3-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="b50e3-148">Type</span></span>        | <span data-ttu-id="b50e3-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="b50e3-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b50e3-150">id</span><span class="sxs-lookup"><span data-stu-id="b50e3-150">id</span></span>|<span data-ttu-id="b50e3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b50e3-151">String</span></span>|<span data-ttu-id="b50e3-152">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="b50e3-152">The document's identifier.</span></span> <span data-ttu-id="b50e3-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b50e3-153">Read-only.</span></span>|
|<span data-ttu-id="b50e3-154">displayName</span><span class="sxs-lookup"><span data-stu-id="b50e3-154">displayName</span></span>|<span data-ttu-id="b50e3-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b50e3-155">String</span></span>|<span data-ttu-id="b50e3-156">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-156">The name of the printer.</span></span>|
|<span data-ttu-id="b50e3-157">fabricante</span><span class="sxs-lookup"><span data-stu-id="b50e3-157">manufacturer</span></span>|<span data-ttu-id="b50e3-158">String</span><span class="sxs-lookup"><span data-stu-id="b50e3-158">String</span></span>|<span data-ttu-id="b50e3-159">O fabricante relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-159">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="b50e3-160">modelo</span><span class="sxs-lookup"><span data-stu-id="b50e3-160">model</span></span>|<span data-ttu-id="b50e3-161">String</span><span class="sxs-lookup"><span data-stu-id="b50e3-161">String</span></span>|<span data-ttu-id="b50e3-162">O nome do modelo relatado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-162">The model name reported by the printer.</span></span>|
|<span data-ttu-id="b50e3-163">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="b50e3-163">registeredDateTime</span></span>|<span data-ttu-id="b50e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b50e3-164">DateTimeOffset</span></span>|<span data-ttu-id="b50e3-165">O DateTimeOffset quando a impressora foi registrada.</span><span class="sxs-lookup"><span data-stu-id="b50e3-165">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="b50e3-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b50e3-166">Read-only.</span></span>|
|<span data-ttu-id="b50e3-167">status</span><span class="sxs-lookup"><span data-stu-id="b50e3-167">status</span></span>|[<span data-ttu-id="b50e3-168">printerStatus</span><span class="sxs-lookup"><span data-stu-id="b50e3-168">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="b50e3-169">O status de processamento da impressora, incluindo erros.</span><span class="sxs-lookup"><span data-stu-id="b50e3-169">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="b50e3-170">isShared</span><span class="sxs-lookup"><span data-stu-id="b50e3-170">isShared</span></span>|<span data-ttu-id="b50e3-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="b50e3-171">Boolean</span></span>|<span data-ttu-id="b50e3-172">True se a impressora é compartilhada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="b50e3-172">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="b50e3-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b50e3-173">Read-only.</span></span>|
|<span data-ttu-id="b50e3-174">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b50e3-174">isAcceptingJobs</span></span>|<span data-ttu-id="b50e3-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="b50e3-175">Boolean</span></span>|<span data-ttu-id="b50e3-176">Se a impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="b50e3-176">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="b50e3-177">localização</span><span class="sxs-lookup"><span data-stu-id="b50e3-177">location</span></span>|[<span data-ttu-id="b50e3-178">printerLocation</span><span class="sxs-lookup"><span data-stu-id="b50e3-178">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="b50e3-179">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-179">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="b50e3-180">defaults</span><span class="sxs-lookup"><span data-stu-id="b50e3-180">defaults</span></span>|[<span data-ttu-id="b50e3-181">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="b50e3-181">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="b50e3-182">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-182">The printer's default print settings.</span></span>|
|<span data-ttu-id="b50e3-183">capabilities</span><span class="sxs-lookup"><span data-stu-id="b50e3-183">capabilities</span></span>|[<span data-ttu-id="b50e3-184">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="b50e3-184">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="b50e3-185">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-185">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b50e3-186">Relações</span><span class="sxs-lookup"><span data-stu-id="b50e3-186">Relationships</span></span>
| <span data-ttu-id="b50e3-187">Relação</span><span class="sxs-lookup"><span data-stu-id="b50e3-187">Relationship</span></span> | <span data-ttu-id="b50e3-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="b50e3-188">Type</span></span>        | <span data-ttu-id="b50e3-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="b50e3-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b50e3-190">jobs</span><span class="sxs-lookup"><span data-stu-id="b50e3-190">jobs</span></span>|<span data-ttu-id="b50e3-191">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b50e3-191">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="b50e3-192">A lista de trabalhos que estão na fila para impressão pela impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-192">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="b50e3-193">shares</span><span class="sxs-lookup"><span data-stu-id="b50e3-193">shares</span></span>|<span data-ttu-id="b50e3-194">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="b50e3-194">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="b50e3-195">A lista de printerShares que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-195">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="b50e3-196">Atualmente, apenas um printerShare pode ser associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-196">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="b50e3-197">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b50e3-197">Read-only.</span></span> <span data-ttu-id="b50e3-198">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b50e3-198">Nullable.</span></span>|
|<span data-ttu-id="b50e3-199">conectores</span><span class="sxs-lookup"><span data-stu-id="b50e3-199">connectors</span></span>|[<span data-ttu-id="b50e3-200">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="b50e3-200">printConnector</span></span>](printconnector.md)|<span data-ttu-id="b50e3-201">Os conectores associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-201">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="b50e3-202">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="b50e3-202">taskTriggers</span></span>|<span data-ttu-id="b50e3-203">coleção [printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="b50e3-203">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="b50e3-204">Uma lista de disparadores de tarefas que estão associados à impressora.</span><span class="sxs-lookup"><span data-stu-id="b50e3-204">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b50e3-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b50e3-205">JSON representation</span></span>

<span data-ttu-id="b50e3-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b50e3-206">The following is a JSON representation of the resource.</span></span>

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


