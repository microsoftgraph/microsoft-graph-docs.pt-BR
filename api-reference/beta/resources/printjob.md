---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 170f413c7607933c2651720c9c9c463f90cf55df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516525"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="55c08-103">Tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="55c08-103">printJob resource type</span></span>

<span data-ttu-id="55c08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55c08-105">Representa um trabalho de impressão que foi ensuado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="55c08-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="55c08-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="55c08-106">Methods</span></span>

| <span data-ttu-id="55c08-107">Método</span><span class="sxs-lookup"><span data-stu-id="55c08-107">Method</span></span>       | <span data-ttu-id="55c08-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55c08-108">Return Type</span></span> | <span data-ttu-id="55c08-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c08-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="55c08-110">Get</span><span class="sxs-lookup"><span data-stu-id="55c08-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="55c08-111">printJob</span><span class="sxs-lookup"><span data-stu-id="55c08-111">printJob</span></span>](printjob.md) | <span data-ttu-id="55c08-112">Ler propriedades e relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="55c08-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="55c08-113">Create</span><span class="sxs-lookup"><span data-stu-id="55c08-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="55c08-114">printJob</span><span class="sxs-lookup"><span data-stu-id="55c08-114">printJob</span></span>](printjob.md) | <span data-ttu-id="55c08-115">Crie um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="55c08-116">Update</span><span class="sxs-lookup"><span data-stu-id="55c08-116">Update</span></span>](../api/printjob-update.md) | [<span data-ttu-id="55c08-117">printJob</span><span class="sxs-lookup"><span data-stu-id="55c08-117">printJob</span></span>](printjob.md) | <span data-ttu-id="55c08-118">Atualizar um objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-118">Update a print job object.</span></span> |
| [<span data-ttu-id="55c08-119">Start</span><span class="sxs-lookup"><span data-stu-id="55c08-119">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="55c08-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55c08-120">None</span></span>|<span data-ttu-id="55c08-121">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-121">Start the print job.</span></span>|
| [<span data-ttu-id="55c08-122">Cancel</span><span class="sxs-lookup"><span data-stu-id="55c08-122">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="55c08-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55c08-123">None</span></span>|<span data-ttu-id="55c08-124">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-124">Cancel the print job.</span></span>|
| <span data-ttu-id="55c08-125">Anular\*\*</span><span class="sxs-lookup"><span data-stu-id="55c08-125">[Abort](../api/printjob-abort.md)</span></span>|<span data-ttu-id="55c08-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55c08-126">None</span></span>|<span data-ttu-id="55c08-127">Aborte o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-127">Abort the print job.</span></span>|
| [<span data-ttu-id="55c08-128">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="55c08-128">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="55c08-129">printJob</span><span class="sxs-lookup"><span data-stu-id="55c08-129">printJob</span></span>](printjob.md) | <span data-ttu-id="55c08-130">Um trabalho de impressão que está na fila para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="55c08-130">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="55c08-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55c08-131">Properties</span></span>
| <span data-ttu-id="55c08-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55c08-132">Property</span></span>     | <span data-ttu-id="55c08-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="55c08-133">Type</span></span>        | <span data-ttu-id="55c08-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c08-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55c08-135">id</span><span class="sxs-lookup"><span data-stu-id="55c08-135">id</span></span>|<span data-ttu-id="55c08-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55c08-136">String</span></span>|<span data-ttu-id="55c08-137">GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="55c08-137">The printer's GUID.</span></span> <span data-ttu-id="55c08-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55c08-138">Read-only.</span></span>|
|<span data-ttu-id="55c08-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55c08-139">createdDateTime</span></span>|<span data-ttu-id="55c08-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55c08-140">DateTimeOffset</span></span>|<span data-ttu-id="55c08-141">DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="55c08-141">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="55c08-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55c08-142">Read-only.</span></span>|
|<span data-ttu-id="55c08-143">status</span><span class="sxs-lookup"><span data-stu-id="55c08-143">status</span></span>|[<span data-ttu-id="55c08-144">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="55c08-144">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="55c08-145">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-145">The status of the print job.</span></span> <span data-ttu-id="55c08-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55c08-146">Read-only.</span></span>|
|<span data-ttu-id="55c08-147">configuração</span><span class="sxs-lookup"><span data-stu-id="55c08-147">configuration</span></span>|[<span data-ttu-id="55c08-148">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="55c08-148">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="55c08-149">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="55c08-149">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="55c08-150">isFetchable</span><span class="sxs-lookup"><span data-stu-id="55c08-150">isFetchable</span></span>|<span data-ttu-id="55c08-151">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="55c08-151">Edm.Boolean</span></span>|<span data-ttu-id="55c08-152">Se true, o documento pode ser buscado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="55c08-152">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="55c08-153">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="55c08-153">redirectedFrom</span></span>|<span data-ttu-id="55c08-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="55c08-154">Edm.String</span></span>|<span data-ttu-id="55c08-155">Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.</span><span class="sxs-lookup"><span data-stu-id="55c08-155">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="55c08-156">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="55c08-156">redirectedTo</span></span>|<span data-ttu-id="55c08-157">Edm.String</span><span class="sxs-lookup"><span data-stu-id="55c08-157">Edm.String</span></span>|<span data-ttu-id="55c08-158">Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="55c08-158">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55c08-159">Relações</span><span class="sxs-lookup"><span data-stu-id="55c08-159">Relationships</span></span>
| <span data-ttu-id="55c08-160">Relação</span><span class="sxs-lookup"><span data-stu-id="55c08-160">Relationship</span></span> | <span data-ttu-id="55c08-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="55c08-161">Type</span></span>        | <span data-ttu-id="55c08-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c08-162">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55c08-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="55c08-163">createdBy</span></span>|[<span data-ttu-id="55c08-164">userIdentity</span><span class="sxs-lookup"><span data-stu-id="55c08-164">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="55c08-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55c08-165">Read-only.</span></span> <span data-ttu-id="55c08-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="55c08-166">Nullable.</span></span>|
|<span data-ttu-id="55c08-167">documents</span><span class="sxs-lookup"><span data-stu-id="55c08-167">documents</span></span>|<span data-ttu-id="55c08-168">[Coleção printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="55c08-168">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="55c08-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55c08-169">Read-only.</span></span>|
|<span data-ttu-id="55c08-170">tarefas</span><span class="sxs-lookup"><span data-stu-id="55c08-170">tasks</span></span>|<span data-ttu-id="55c08-171">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="55c08-171">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="55c08-172">Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="55c08-172">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55c08-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55c08-173">JSON representation</span></span>

<span data-ttu-id="55c08-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55c08-174">The following is a JSON representation of the resource.</span></span>

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

