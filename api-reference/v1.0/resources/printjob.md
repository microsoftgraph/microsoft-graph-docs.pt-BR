---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3115164fcc15ef6c2133ef3616624af9141da1af
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517039"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="f1757-103">Tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="f1757-103">printJob resource type</span></span>

<span data-ttu-id="f1757-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f1757-105">Representa um trabalho de impressão que foi ensuado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="f1757-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="f1757-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1757-106">Methods</span></span>
| <span data-ttu-id="f1757-107">Método</span><span class="sxs-lookup"><span data-stu-id="f1757-107">Method</span></span>       | <span data-ttu-id="f1757-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1757-108">Return Type</span></span> | <span data-ttu-id="f1757-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1757-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f1757-110">Get</span><span class="sxs-lookup"><span data-stu-id="f1757-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="f1757-111">printJob</span><span class="sxs-lookup"><span data-stu-id="f1757-111">printJob</span></span>](printjob.md) | <span data-ttu-id="f1757-112">Ler propriedades e relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="f1757-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="f1757-113">Create</span><span class="sxs-lookup"><span data-stu-id="f1757-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="f1757-114">printJob</span><span class="sxs-lookup"><span data-stu-id="f1757-114">printJob</span></span>](printjob.md) | <span data-ttu-id="f1757-115">Crie um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="f1757-116">Update</span><span class="sxs-lookup"><span data-stu-id="f1757-116">Update</span></span>](../api/printjob-update.md) | [<span data-ttu-id="f1757-117">printJob</span><span class="sxs-lookup"><span data-stu-id="f1757-117">printJob</span></span>](printjob.md) | <span data-ttu-id="f1757-118">Atualizar um objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-118">Update a print job object.</span></span> |
| [<span data-ttu-id="f1757-119">Start</span><span class="sxs-lookup"><span data-stu-id="f1757-119">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="f1757-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1757-120">None</span></span>|<span data-ttu-id="f1757-121">Iniciar o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-121">Start the print job.</span></span>|
| [<span data-ttu-id="f1757-122">Cancel</span><span class="sxs-lookup"><span data-stu-id="f1757-122">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="f1757-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1757-123">None</span></span>|<span data-ttu-id="f1757-124">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-124">Cancel the print job.</span></span>|
| <span data-ttu-id="f1757-125">Anular\*\*</span><span class="sxs-lookup"><span data-stu-id="f1757-125">[Abort](../api/printjob-abort.md)</span></span>|<span data-ttu-id="f1757-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1757-126">None</span></span>|<span data-ttu-id="f1757-127">Aborte o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-127">Abort the print job.</span></span>|
| [<span data-ttu-id="f1757-128">Redirecionar (para outra impressora)</span><span class="sxs-lookup"><span data-stu-id="f1757-128">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="f1757-129">printJob</span><span class="sxs-lookup"><span data-stu-id="f1757-129">printJob</span></span>](printjob.md) | <span data-ttu-id="f1757-130">Um trabalho de impressão que está na fila para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="f1757-130">A print job that is queued for the destination printer.</span></span> |


## <a name="properties"></a><span data-ttu-id="f1757-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1757-131">Properties</span></span>
|<span data-ttu-id="f1757-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1757-132">Property</span></span>|<span data-ttu-id="f1757-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1757-133">Type</span></span>|<span data-ttu-id="f1757-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1757-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1757-135">id</span><span class="sxs-lookup"><span data-stu-id="f1757-135">id</span></span>|<span data-ttu-id="f1757-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1757-136">String</span></span>|<span data-ttu-id="f1757-137">GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="f1757-137">The printer's GUID.</span></span> <span data-ttu-id="f1757-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1757-138">Read-only.</span></span>|
|<span data-ttu-id="f1757-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1757-139">createdDateTime</span></span>|<span data-ttu-id="f1757-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1757-140">DateTimeOffset</span></span>|<span data-ttu-id="f1757-141">DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="f1757-141">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="f1757-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1757-142">Read-only.</span></span>|
|<span data-ttu-id="f1757-143">status</span><span class="sxs-lookup"><span data-stu-id="f1757-143">status</span></span>|[<span data-ttu-id="f1757-144">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="f1757-144">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="f1757-145">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-145">The status of the print job.</span></span> <span data-ttu-id="f1757-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1757-146">Read-only.</span></span>|
|<span data-ttu-id="f1757-147">configuração</span><span class="sxs-lookup"><span data-stu-id="f1757-147">configuration</span></span>|[<span data-ttu-id="f1757-148">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1757-148">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="f1757-149">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="f1757-149">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="f1757-150">isFetchable</span><span class="sxs-lookup"><span data-stu-id="f1757-150">isFetchable</span></span>|<span data-ttu-id="f1757-151">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f1757-151">Edm.Boolean</span></span>|<span data-ttu-id="f1757-152">Se true, o documento pode ser buscado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="f1757-152">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="f1757-153">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="f1757-153">redirectedFrom</span></span>|<span data-ttu-id="f1757-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="f1757-154">Edm.String</span></span>|<span data-ttu-id="f1757-155">Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.</span><span class="sxs-lookup"><span data-stu-id="f1757-155">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="f1757-156">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="f1757-156">redirectedTo</span></span>|<span data-ttu-id="f1757-157">Edm.String</span><span class="sxs-lookup"><span data-stu-id="f1757-157">Edm.String</span></span>|<span data-ttu-id="f1757-158">Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.</span><span class="sxs-lookup"><span data-stu-id="f1757-158">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|
|<span data-ttu-id="f1757-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="f1757-159">createdBy</span></span>|[<span data-ttu-id="f1757-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f1757-160">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f1757-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1757-161">Read-only.</span></span> <span data-ttu-id="f1757-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f1757-162">Nullable.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1757-163">Relações</span><span class="sxs-lookup"><span data-stu-id="f1757-163">Relationships</span></span>
|<span data-ttu-id="f1757-164">Relação</span><span class="sxs-lookup"><span data-stu-id="f1757-164">Relationship</span></span>|<span data-ttu-id="f1757-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1757-165">Type</span></span>|<span data-ttu-id="f1757-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1757-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1757-167">documents</span><span class="sxs-lookup"><span data-stu-id="f1757-167">documents</span></span>|<span data-ttu-id="f1757-168">[Coleção printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="f1757-168">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="f1757-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1757-169">Read-only.</span></span>|
|<span data-ttu-id="f1757-170">tarefas</span><span class="sxs-lookup"><span data-stu-id="f1757-170">tasks</span></span>|<span data-ttu-id="f1757-171">[Coleção printTask](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="f1757-171">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="f1757-172">Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="f1757-172">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1757-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1757-173">JSON representation</span></span>
<span data-ttu-id="f1757-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1757-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration"
  },
  "redirectedTo": "String",
  "redirectedFrom": "String",
  "isFetchable": "Boolean"
}
```

