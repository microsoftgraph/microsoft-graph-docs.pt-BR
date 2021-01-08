---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 43b08c39715c9984a1692c0bcb823881be4ab4d1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784826"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="52d11-103">Tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="52d11-103">printJob resource type</span></span>

<span data-ttu-id="52d11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52d11-105">Representa um trabalho de impressão que foi ensuado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="52d11-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="52d11-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52d11-106">Methods</span></span>

| <span data-ttu-id="52d11-107">Método</span><span class="sxs-lookup"><span data-stu-id="52d11-107">Method</span></span>       | <span data-ttu-id="52d11-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52d11-108">Return Type</span></span> | <span data-ttu-id="52d11-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d11-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52d11-110">Get</span><span class="sxs-lookup"><span data-stu-id="52d11-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="52d11-111">printJob</span><span class="sxs-lookup"><span data-stu-id="52d11-111">printJob</span></span>](printjob.md) | <span data-ttu-id="52d11-112">Leia as propriedades e os relacionamentos do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="52d11-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="52d11-113">Create</span><span class="sxs-lookup"><span data-stu-id="52d11-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="52d11-114">printJob</span><span class="sxs-lookup"><span data-stu-id="52d11-114">printJob</span></span>](printjob.md) | <span data-ttu-id="52d11-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="52d11-116">Start</span><span class="sxs-lookup"><span data-stu-id="52d11-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="52d11-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52d11-117">None</span></span>|<span data-ttu-id="52d11-118">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-118">Start the print job.</span></span>|
| [<span data-ttu-id="52d11-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="52d11-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="52d11-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52d11-120">None</span></span>|<span data-ttu-id="52d11-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-121">Cancel the print job.</span></span>|
| <span data-ttu-id="52d11-122">Anular\*\*</span><span class="sxs-lookup"><span data-stu-id="52d11-122">[Abort](../api/printjob-abort.md)</span></span>|<span data-ttu-id="52d11-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52d11-123">None</span></span>|<span data-ttu-id="52d11-124">Anula o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-124">Abort the print job.</span></span>|
| [<span data-ttu-id="52d11-125">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="52d11-125">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="52d11-126">printJob</span><span class="sxs-lookup"><span data-stu-id="52d11-126">printJob</span></span>](printjob.md) | <span data-ttu-id="52d11-127">Um trabalho de impressão que está na fila para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="52d11-127">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="52d11-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52d11-128">Properties</span></span>
| <span data-ttu-id="52d11-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52d11-129">Property</span></span>     | <span data-ttu-id="52d11-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="52d11-130">Type</span></span>        | <span data-ttu-id="52d11-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d11-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52d11-132">id</span><span class="sxs-lookup"><span data-stu-id="52d11-132">id</span></span>|<span data-ttu-id="52d11-133">String</span><span class="sxs-lookup"><span data-stu-id="52d11-133">String</span></span>|<span data-ttu-id="52d11-134">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="52d11-134">The printer's GUID.</span></span> <span data-ttu-id="52d11-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52d11-135">Read-only.</span></span>|
|<span data-ttu-id="52d11-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52d11-136">createdDateTime</span></span>|<span data-ttu-id="52d11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52d11-137">DateTimeOffset</span></span>|<span data-ttu-id="52d11-138">DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="52d11-138">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="52d11-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52d11-139">Read-only.</span></span>|
|<span data-ttu-id="52d11-140">status</span><span class="sxs-lookup"><span data-stu-id="52d11-140">status</span></span>|[<span data-ttu-id="52d11-141">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="52d11-141">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="52d11-142">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-142">The status of the print job.</span></span> <span data-ttu-id="52d11-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52d11-143">Read-only.</span></span>|
|<span data-ttu-id="52d11-144">configuração</span><span class="sxs-lookup"><span data-stu-id="52d11-144">configuration</span></span>|[<span data-ttu-id="52d11-145">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="52d11-145">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="52d11-146">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="52d11-146">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="52d11-147">isFetchable</span><span class="sxs-lookup"><span data-stu-id="52d11-147">isFetchable</span></span>|<span data-ttu-id="52d11-148">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="52d11-148">Edm.Boolean</span></span>|<span data-ttu-id="52d11-149">Se verdadeiro, o documento pode ser buscado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="52d11-149">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="52d11-150">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="52d11-150">redirectedFrom</span></span>|<span data-ttu-id="52d11-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="52d11-151">Edm.String</span></span>|<span data-ttu-id="52d11-152">Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.</span><span class="sxs-lookup"><span data-stu-id="52d11-152">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="52d11-153">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="52d11-153">redirectedTo</span></span>|<span data-ttu-id="52d11-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="52d11-154">Edm.String</span></span>|<span data-ttu-id="52d11-155">Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="52d11-155">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d11-156">Relações</span><span class="sxs-lookup"><span data-stu-id="52d11-156">Relationships</span></span>
| <span data-ttu-id="52d11-157">Relação</span><span class="sxs-lookup"><span data-stu-id="52d11-157">Relationship</span></span> | <span data-ttu-id="52d11-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="52d11-158">Type</span></span>        | <span data-ttu-id="52d11-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d11-159">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52d11-160">createdBy</span><span class="sxs-lookup"><span data-stu-id="52d11-160">createdBy</span></span>|[<span data-ttu-id="52d11-161">userIdentity</span><span class="sxs-lookup"><span data-stu-id="52d11-161">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="52d11-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52d11-162">Read-only.</span></span> <span data-ttu-id="52d11-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="52d11-163">Nullable.</span></span>|
|<span data-ttu-id="52d11-164">documentos</span><span class="sxs-lookup"><span data-stu-id="52d11-164">documents</span></span>|<span data-ttu-id="52d11-165">[Coleção printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="52d11-165">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="52d11-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52d11-166">Read-only.</span></span>|
|<span data-ttu-id="52d11-167">tarefas</span><span class="sxs-lookup"><span data-stu-id="52d11-167">tasks</span></span>|<span data-ttu-id="52d11-168">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="52d11-168">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="52d11-169">Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="52d11-169">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52d11-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52d11-170">JSON representation</span></span>

<span data-ttu-id="52d11-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52d11-171">The following is a JSON representation of the resource.</span></span>

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

