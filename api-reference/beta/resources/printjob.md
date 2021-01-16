---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5124f3123331c4889f5e16110109938e7f264925
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883029"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="3553a-103">Tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="3553a-103">printJob resource type</span></span>

<span data-ttu-id="3553a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3553a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3553a-105">Representa um trabalho de impressão que foi ensuado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="3553a-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="3553a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3553a-106">Methods</span></span>

| <span data-ttu-id="3553a-107">Método</span><span class="sxs-lookup"><span data-stu-id="3553a-107">Method</span></span>       | <span data-ttu-id="3553a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3553a-108">Return Type</span></span> | <span data-ttu-id="3553a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3553a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3553a-110">Get</span><span class="sxs-lookup"><span data-stu-id="3553a-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="3553a-111">printJob</span><span class="sxs-lookup"><span data-stu-id="3553a-111">printJob</span></span>](printjob.md) | <span data-ttu-id="3553a-112">Leia as propriedades e os relacionamentos do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="3553a-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="3553a-113">Create</span><span class="sxs-lookup"><span data-stu-id="3553a-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="3553a-114">printJob</span><span class="sxs-lookup"><span data-stu-id="3553a-114">printJob</span></span>](printjob.md) | <span data-ttu-id="3553a-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="3553a-116">Start</span><span class="sxs-lookup"><span data-stu-id="3553a-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="3553a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3553a-117">None</span></span>|<span data-ttu-id="3553a-118">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-118">Start the print job.</span></span>|
| [<span data-ttu-id="3553a-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="3553a-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="3553a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3553a-120">None</span></span>|<span data-ttu-id="3553a-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-121">Cancel the print job.</span></span>|
| <span data-ttu-id="3553a-122">Anular\*\*</span><span class="sxs-lookup"><span data-stu-id="3553a-122">[Abort](../api/printjob-abort.md)</span></span>|<span data-ttu-id="3553a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3553a-123">None</span></span>|<span data-ttu-id="3553a-124">Anula o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-124">Abort the print job.</span></span>|
| [<span data-ttu-id="3553a-125">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="3553a-125">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="3553a-126">printJob</span><span class="sxs-lookup"><span data-stu-id="3553a-126">printJob</span></span>](printjob.md) | <span data-ttu-id="3553a-127">Um trabalho de impressão que está na fila para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="3553a-127">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="3553a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3553a-128">Properties</span></span>
| <span data-ttu-id="3553a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3553a-129">Property</span></span>     | <span data-ttu-id="3553a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3553a-130">Type</span></span>        | <span data-ttu-id="3553a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3553a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3553a-132">id</span><span class="sxs-lookup"><span data-stu-id="3553a-132">id</span></span>|<span data-ttu-id="3553a-133">String</span><span class="sxs-lookup"><span data-stu-id="3553a-133">String</span></span>|<span data-ttu-id="3553a-134">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="3553a-134">The printer's GUID.</span></span> <span data-ttu-id="3553a-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3553a-135">Read-only.</span></span>|
|<span data-ttu-id="3553a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3553a-136">createdDateTime</span></span>|<span data-ttu-id="3553a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3553a-137">DateTimeOffset</span></span>|<span data-ttu-id="3553a-138">DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="3553a-138">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="3553a-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3553a-139">Read-only.</span></span>|
|<span data-ttu-id="3553a-140">status</span><span class="sxs-lookup"><span data-stu-id="3553a-140">status</span></span>|[<span data-ttu-id="3553a-141">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="3553a-141">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="3553a-142">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-142">The status of the print job.</span></span> <span data-ttu-id="3553a-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3553a-143">Read-only.</span></span>|
|<span data-ttu-id="3553a-144">configuração</span><span class="sxs-lookup"><span data-stu-id="3553a-144">configuration</span></span>|[<span data-ttu-id="3553a-145">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="3553a-145">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="3553a-146">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="3553a-146">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="3553a-147">isFetchable</span><span class="sxs-lookup"><span data-stu-id="3553a-147">isFetchable</span></span>|<span data-ttu-id="3553a-148">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="3553a-148">Edm.Boolean</span></span>|<span data-ttu-id="3553a-149">Se verdadeiro, o documento pode ser buscado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="3553a-149">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="3553a-150">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="3553a-150">redirectedFrom</span></span>|<span data-ttu-id="3553a-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="3553a-151">Edm.String</span></span>|<span data-ttu-id="3553a-152">Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.</span><span class="sxs-lookup"><span data-stu-id="3553a-152">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="3553a-153">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="3553a-153">redirectedTo</span></span>|<span data-ttu-id="3553a-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="3553a-154">Edm.String</span></span>|<span data-ttu-id="3553a-155">Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="3553a-155">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3553a-156">Relações</span><span class="sxs-lookup"><span data-stu-id="3553a-156">Relationships</span></span>
| <span data-ttu-id="3553a-157">Relação</span><span class="sxs-lookup"><span data-stu-id="3553a-157">Relationship</span></span> | <span data-ttu-id="3553a-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="3553a-158">Type</span></span>        | <span data-ttu-id="3553a-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="3553a-159">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3553a-160">createdBy</span><span class="sxs-lookup"><span data-stu-id="3553a-160">createdBy</span></span>|[<span data-ttu-id="3553a-161">userIdentity</span><span class="sxs-lookup"><span data-stu-id="3553a-161">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="3553a-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3553a-162">Read-only.</span></span> <span data-ttu-id="3553a-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3553a-163">Nullable.</span></span>|
|<span data-ttu-id="3553a-164">documentos</span><span class="sxs-lookup"><span data-stu-id="3553a-164">documents</span></span>|<span data-ttu-id="3553a-165">[Coleção printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="3553a-165">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="3553a-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3553a-166">Read-only.</span></span>|
|<span data-ttu-id="3553a-167">tarefas</span><span class="sxs-lookup"><span data-stu-id="3553a-167">tasks</span></span>|<span data-ttu-id="3553a-168">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="3553a-168">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="3553a-169">Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3553a-169">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3553a-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3553a-170">JSON representation</span></span>

<span data-ttu-id="3553a-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3553a-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

