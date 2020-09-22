---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2c0a1bdb4ec3ebe3c87b5b40595d30cf9108c5bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048733"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="2acba-103">tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="2acba-103">printJob resource type</span></span>

<span data-ttu-id="2acba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2acba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2acba-105">Representa um trabalho de impressão que foi enfileirado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="2acba-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="2acba-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2acba-106">Methods</span></span>

| <span data-ttu-id="2acba-107">Método</span><span class="sxs-lookup"><span data-stu-id="2acba-107">Method</span></span>       | <span data-ttu-id="2acba-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2acba-108">Return Type</span></span> | <span data-ttu-id="2acba-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acba-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2acba-110">Get</span><span class="sxs-lookup"><span data-stu-id="2acba-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="2acba-111">Impressão</span><span class="sxs-lookup"><span data-stu-id="2acba-111">printJob</span></span>](printjob.md) | <span data-ttu-id="2acba-112">Leia as propriedades e as relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="2acba-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="2acba-113">Criar</span><span class="sxs-lookup"><span data-stu-id="2acba-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="2acba-114">Impressão</span><span class="sxs-lookup"><span data-stu-id="2acba-114">printJob</span></span>](printjob.md) | <span data-ttu-id="2acba-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="2acba-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="2acba-116">Start</span><span class="sxs-lookup"><span data-stu-id="2acba-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="2acba-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2acba-117">None</span></span>|<span data-ttu-id="2acba-118">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="2acba-118">Start the print job.</span></span>|
| [<span data-ttu-id="2acba-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="2acba-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="2acba-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2acba-120">None</span></span>|<span data-ttu-id="2acba-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="2acba-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="2acba-122">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="2acba-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="2acba-123">Impressão</span><span class="sxs-lookup"><span data-stu-id="2acba-123">printJob</span></span>](printjob.md) | <span data-ttu-id="2acba-124">Um trabalho de impressão que está na fila da impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="2acba-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="2acba-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2acba-125">Properties</span></span>
| <span data-ttu-id="2acba-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2acba-126">Property</span></span>     | <span data-ttu-id="2acba-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2acba-127">Type</span></span>        | <span data-ttu-id="2acba-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acba-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2acba-129">id</span><span class="sxs-lookup"><span data-stu-id="2acba-129">id</span></span>|<span data-ttu-id="2acba-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2acba-130">String</span></span>|<span data-ttu-id="2acba-131">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="2acba-131">The printer's GUID.</span></span> <span data-ttu-id="2acba-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acba-132">Read-only.</span></span>|
|<span data-ttu-id="2acba-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2acba-133">createdDateTime</span></span>|<span data-ttu-id="2acba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2acba-134">DateTimeOffset</span></span>|<span data-ttu-id="2acba-135">O DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="2acba-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="2acba-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acba-136">Read-only.</span></span>|
|<span data-ttu-id="2acba-137">status</span><span class="sxs-lookup"><span data-stu-id="2acba-137">status</span></span>|[<span data-ttu-id="2acba-138">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="2acba-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="2acba-139">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="2acba-139">The status of the print job.</span></span> <span data-ttu-id="2acba-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acba-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2acba-141">Relações</span><span class="sxs-lookup"><span data-stu-id="2acba-141">Relationships</span></span>
| <span data-ttu-id="2acba-142">Relação</span><span class="sxs-lookup"><span data-stu-id="2acba-142">Relationship</span></span> | <span data-ttu-id="2acba-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="2acba-143">Type</span></span>        | <span data-ttu-id="2acba-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acba-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2acba-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="2acba-145">createdBy</span></span>|[<span data-ttu-id="2acba-146">userIdentity</span><span class="sxs-lookup"><span data-stu-id="2acba-146">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="2acba-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acba-147">Read-only.</span></span> <span data-ttu-id="2acba-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2acba-148">Nullable.</span></span>|
|<span data-ttu-id="2acba-149">documentos</span><span class="sxs-lookup"><span data-stu-id="2acba-149">documents</span></span>|<span data-ttu-id="2acba-150">coleção [AddDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="2acba-150">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="2acba-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acba-151">Read-only.</span></span>|
|<span data-ttu-id="2acba-152">tarefas</span><span class="sxs-lookup"><span data-stu-id="2acba-152">tasks</span></span>|<span data-ttu-id="2acba-153">coleção [multitask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="2acba-153">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="2acba-154">Uma lista de [multitarefas](printtask.md) que foram acionadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="2acba-154">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2acba-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2acba-155">JSON representation</span></span>

<span data-ttu-id="2acba-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2acba-156">The following is a JSON representation of the resource.</span></span>

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
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
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

