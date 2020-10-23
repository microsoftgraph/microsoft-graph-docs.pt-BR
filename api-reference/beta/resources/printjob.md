---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7810c8cd864020c42de4482deea67620950f6cf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726289"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="589c5-103">tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="589c5-103">printJob resource type</span></span>

<span data-ttu-id="589c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="589c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="589c5-105">Representa um trabalho de impressão que foi enfileirado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="589c5-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="589c5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="589c5-106">Methods</span></span>

| <span data-ttu-id="589c5-107">Método</span><span class="sxs-lookup"><span data-stu-id="589c5-107">Method</span></span>       | <span data-ttu-id="589c5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="589c5-108">Return Type</span></span> | <span data-ttu-id="589c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="589c5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="589c5-110">Get</span><span class="sxs-lookup"><span data-stu-id="589c5-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="589c5-111">Impressão</span><span class="sxs-lookup"><span data-stu-id="589c5-111">printJob</span></span>](printjob.md) | <span data-ttu-id="589c5-112">Leia as propriedades e as relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="589c5-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="589c5-113">Create</span><span class="sxs-lookup"><span data-stu-id="589c5-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="589c5-114">Impressão</span><span class="sxs-lookup"><span data-stu-id="589c5-114">printJob</span></span>](printjob.md) | <span data-ttu-id="589c5-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="589c5-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="589c5-116">Start</span><span class="sxs-lookup"><span data-stu-id="589c5-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="589c5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="589c5-117">None</span></span>|<span data-ttu-id="589c5-118">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="589c5-118">Start the print job.</span></span>|
| [<span data-ttu-id="589c5-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="589c5-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="589c5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="589c5-120">None</span></span>|<span data-ttu-id="589c5-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="589c5-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="589c5-122">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="589c5-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="589c5-123">Impressão</span><span class="sxs-lookup"><span data-stu-id="589c5-123">printJob</span></span>](printjob.md) | <span data-ttu-id="589c5-124">Um trabalho de impressão que está na fila da impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="589c5-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="589c5-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="589c5-125">Properties</span></span>
| <span data-ttu-id="589c5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="589c5-126">Property</span></span>     | <span data-ttu-id="589c5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="589c5-127">Type</span></span>        | <span data-ttu-id="589c5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="589c5-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="589c5-129">id</span><span class="sxs-lookup"><span data-stu-id="589c5-129">id</span></span>|<span data-ttu-id="589c5-130">String</span><span class="sxs-lookup"><span data-stu-id="589c5-130">String</span></span>|<span data-ttu-id="589c5-131">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="589c5-131">The printer's GUID.</span></span> <span data-ttu-id="589c5-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="589c5-132">Read-only.</span></span>|
|<span data-ttu-id="589c5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="589c5-133">createdDateTime</span></span>|<span data-ttu-id="589c5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="589c5-134">DateTimeOffset</span></span>|<span data-ttu-id="589c5-135">O DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="589c5-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="589c5-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="589c5-136">Read-only.</span></span>|
|<span data-ttu-id="589c5-137">status</span><span class="sxs-lookup"><span data-stu-id="589c5-137">status</span></span>|[<span data-ttu-id="589c5-138">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="589c5-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="589c5-139">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="589c5-139">The status of the print job.</span></span> <span data-ttu-id="589c5-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="589c5-140">Read-only.</span></span>|
|<span data-ttu-id="589c5-141">configuration</span><span class="sxs-lookup"><span data-stu-id="589c5-141">configuration</span></span>|[<span data-ttu-id="589c5-142">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="589c5-142">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="589c5-143">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="589c5-143">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="589c5-144">isfetchable</span><span class="sxs-lookup"><span data-stu-id="589c5-144">isFetchable</span></span>|<span data-ttu-id="589c5-145">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="589c5-145">Edm.Boolean</span></span>|<span data-ttu-id="589c5-146">Se true, o documento pode ser obtido pela impressora.</span><span class="sxs-lookup"><span data-stu-id="589c5-146">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="589c5-147">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="589c5-147">redirectedFrom</span></span>|<span data-ttu-id="589c5-148">Edm.String</span><span class="sxs-lookup"><span data-stu-id="589c5-148">Edm.String</span></span>|<span data-ttu-id="589c5-149">Contém a URL do trabalho de origem, se o trabalho foi Redirecionado de outra impressora.</span><span class="sxs-lookup"><span data-stu-id="589c5-149">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="589c5-150">redirecionato</span><span class="sxs-lookup"><span data-stu-id="589c5-150">redirectedTo</span></span>|<span data-ttu-id="589c5-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="589c5-151">Edm.String</span></span>|<span data-ttu-id="589c5-152">Contém a URL do trabalho de destino, se o trabalho foi redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="589c5-152">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="589c5-153">Relações</span><span class="sxs-lookup"><span data-stu-id="589c5-153">Relationships</span></span>
| <span data-ttu-id="589c5-154">Relação</span><span class="sxs-lookup"><span data-stu-id="589c5-154">Relationship</span></span> | <span data-ttu-id="589c5-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="589c5-155">Type</span></span>        | <span data-ttu-id="589c5-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="589c5-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="589c5-157">createdBy</span><span class="sxs-lookup"><span data-stu-id="589c5-157">createdBy</span></span>|[<span data-ttu-id="589c5-158">userIdentity</span><span class="sxs-lookup"><span data-stu-id="589c5-158">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="589c5-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="589c5-159">Read-only.</span></span> <span data-ttu-id="589c5-160">Anulável.</span><span class="sxs-lookup"><span data-stu-id="589c5-160">Nullable.</span></span>|
|<span data-ttu-id="589c5-161">documentos</span><span class="sxs-lookup"><span data-stu-id="589c5-161">documents</span></span>|<span data-ttu-id="589c5-162">coleção [AddDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="589c5-162">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="589c5-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="589c5-163">Read-only.</span></span>|
|<span data-ttu-id="589c5-164">tarefas</span><span class="sxs-lookup"><span data-stu-id="589c5-164">tasks</span></span>|<span data-ttu-id="589c5-165">coleção [multitask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="589c5-165">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="589c5-166">Uma lista de [multitarefas](printtask.md) que foram acionadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="589c5-166">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="589c5-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="589c5-167">JSON representation</span></span>

<span data-ttu-id="589c5-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="589c5-168">The following is a JSON representation of the resource.</span></span>

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

