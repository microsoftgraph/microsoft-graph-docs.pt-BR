---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0d46263e5f393362cec155a9be3e2e5a54c3dfec
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091519"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="8fda2-103">tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="8fda2-103">printJob resource type</span></span>

<span data-ttu-id="8fda2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fda2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fda2-105">Representa um trabalho de impressão que foi enfileirado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="8fda2-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="8fda2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8fda2-106">Methods</span></span>

| <span data-ttu-id="8fda2-107">Método</span><span class="sxs-lookup"><span data-stu-id="8fda2-107">Method</span></span>       | <span data-ttu-id="8fda2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8fda2-108">Return Type</span></span> | <span data-ttu-id="8fda2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fda2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8fda2-110">Get</span><span class="sxs-lookup"><span data-stu-id="8fda2-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="8fda2-111">Impressão</span><span class="sxs-lookup"><span data-stu-id="8fda2-111">printJob</span></span>](printjob.md) | <span data-ttu-id="8fda2-112">Leia as propriedades e as relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="8fda2-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="8fda2-113">Criar</span><span class="sxs-lookup"><span data-stu-id="8fda2-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="8fda2-114">Impressão</span><span class="sxs-lookup"><span data-stu-id="8fda2-114">printJob</span></span>](printjob.md) | <span data-ttu-id="8fda2-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8fda2-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="8fda2-116">Start</span><span class="sxs-lookup"><span data-stu-id="8fda2-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="8fda2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fda2-117">None</span></span>|<span data-ttu-id="8fda2-118">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8fda2-118">Start the print job.</span></span>|
| [<span data-ttu-id="8fda2-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="8fda2-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="8fda2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fda2-120">None</span></span>|<span data-ttu-id="8fda2-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8fda2-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="8fda2-122">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="8fda2-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="8fda2-123">Impressão</span><span class="sxs-lookup"><span data-stu-id="8fda2-123">printJob</span></span>](printjob.md) | <span data-ttu-id="8fda2-124">Um trabalho de impressão que está na fila da impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="8fda2-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="8fda2-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fda2-125">Properties</span></span>
| <span data-ttu-id="8fda2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fda2-126">Property</span></span>     | <span data-ttu-id="8fda2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fda2-127">Type</span></span>        | <span data-ttu-id="8fda2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fda2-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8fda2-129">id</span><span class="sxs-lookup"><span data-stu-id="8fda2-129">id</span></span>|<span data-ttu-id="8fda2-130">String</span><span class="sxs-lookup"><span data-stu-id="8fda2-130">String</span></span>|<span data-ttu-id="8fda2-131">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="8fda2-131">The printer's GUID.</span></span> <span data-ttu-id="8fda2-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fda2-132">Read-only.</span></span>|
|<span data-ttu-id="8fda2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fda2-133">createdDateTime</span></span>|<span data-ttu-id="8fda2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fda2-134">DateTimeOffset</span></span>|<span data-ttu-id="8fda2-135">O DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="8fda2-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="8fda2-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fda2-136">Read-only.</span></span>|
|<span data-ttu-id="8fda2-137">status</span><span class="sxs-lookup"><span data-stu-id="8fda2-137">status</span></span>|[<span data-ttu-id="8fda2-138">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="8fda2-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="8fda2-139">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8fda2-139">The status of the print job.</span></span> <span data-ttu-id="8fda2-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fda2-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fda2-141">Relações</span><span class="sxs-lookup"><span data-stu-id="8fda2-141">Relationships</span></span>
| <span data-ttu-id="8fda2-142">Relação</span><span class="sxs-lookup"><span data-stu-id="8fda2-142">Relationship</span></span> | <span data-ttu-id="8fda2-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fda2-143">Type</span></span>        | <span data-ttu-id="8fda2-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fda2-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8fda2-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="8fda2-145">createdBy</span></span>|[<span data-ttu-id="8fda2-146">userIdentity</span><span class="sxs-lookup"><span data-stu-id="8fda2-146">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="8fda2-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fda2-147">Read-only.</span></span> <span data-ttu-id="8fda2-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8fda2-148">Nullable.</span></span>|
|<span data-ttu-id="8fda2-149">documentos</span><span class="sxs-lookup"><span data-stu-id="8fda2-149">documents</span></span>|<span data-ttu-id="8fda2-150">coleção [AddDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="8fda2-150">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="8fda2-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fda2-151">Read-only.</span></span>|
|<span data-ttu-id="8fda2-152">tarefas</span><span class="sxs-lookup"><span data-stu-id="8fda2-152">tasks</span></span>|<span data-ttu-id="8fda2-153">coleção [multitask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="8fda2-153">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="8fda2-154">Uma lista de [multitarefas](printtask.md) que foram acionadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8fda2-154">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fda2-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fda2-155">JSON representation</span></span>

<span data-ttu-id="8fda2-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8fda2-156">The following is a JSON representation of the resource.</span></span>

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