---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eff75fba2c9993275c277877fedec7705021c49
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895478"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="e8d22-103">tipo de recurso printJob</span><span class="sxs-lookup"><span data-stu-id="e8d22-103">printJob resource type</span></span>

<span data-ttu-id="e8d22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8d22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8d22-105">Representa um trabalho de impressão que foi enfileirado para uma impressora.</span><span class="sxs-lookup"><span data-stu-id="e8d22-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="e8d22-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e8d22-106">Methods</span></span>

| <span data-ttu-id="e8d22-107">Método</span><span class="sxs-lookup"><span data-stu-id="e8d22-107">Method</span></span>       | <span data-ttu-id="e8d22-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e8d22-108">Return Type</span></span> | <span data-ttu-id="e8d22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d22-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e8d22-110">Get</span><span class="sxs-lookup"><span data-stu-id="e8d22-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="e8d22-111">Impressão</span><span class="sxs-lookup"><span data-stu-id="e8d22-111">printJob</span></span>](printjob.md) | <span data-ttu-id="e8d22-112">Leia as propriedades e as relações do objeto printJob.</span><span class="sxs-lookup"><span data-stu-id="e8d22-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="e8d22-113">Create</span><span class="sxs-lookup"><span data-stu-id="e8d22-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="e8d22-114">Impressão</span><span class="sxs-lookup"><span data-stu-id="e8d22-114">printJob</span></span>](printjob.md) | <span data-ttu-id="e8d22-115">Criar um novo objeto de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e8d22-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="e8d22-116">Start</span><span class="sxs-lookup"><span data-stu-id="e8d22-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="e8d22-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8d22-117">None</span></span>|<span data-ttu-id="e8d22-118">Inicie o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e8d22-118">Start the print job.</span></span>|
| [<span data-ttu-id="e8d22-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="e8d22-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="e8d22-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8d22-120">None</span></span>|<span data-ttu-id="e8d22-121">Cancele o trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e8d22-121">Cancel the print job.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8d22-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8d22-122">Properties</span></span>
| <span data-ttu-id="e8d22-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8d22-123">Property</span></span>     | <span data-ttu-id="e8d22-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8d22-124">Type</span></span>        | <span data-ttu-id="e8d22-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d22-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8d22-126">id</span><span class="sxs-lookup"><span data-stu-id="e8d22-126">id</span></span>|<span data-ttu-id="e8d22-127">String</span><span class="sxs-lookup"><span data-stu-id="e8d22-127">String</span></span>|<span data-ttu-id="e8d22-128">O GUID da impressora.</span><span class="sxs-lookup"><span data-stu-id="e8d22-128">The printer's GUID.</span></span> <span data-ttu-id="e8d22-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8d22-129">Read-only.</span></span>|
|<span data-ttu-id="e8d22-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8d22-130">createdDateTime</span></span>|<span data-ttu-id="e8d22-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8d22-131">DateTimeOffset</span></span>|<span data-ttu-id="e8d22-132">O DateTimeOffset quando o trabalho foi criado.</span><span class="sxs-lookup"><span data-stu-id="e8d22-132">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="e8d22-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8d22-133">Read-only.</span></span>|
|<span data-ttu-id="e8d22-134">status</span><span class="sxs-lookup"><span data-stu-id="e8d22-134">status</span></span>|[<span data-ttu-id="e8d22-135">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="e8d22-135">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="e8d22-136">O status do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e8d22-136">The status of the print job.</span></span> <span data-ttu-id="e8d22-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8d22-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8d22-138">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="e8d22-138">Relationships</span></span>
| <span data-ttu-id="e8d22-139">Relação</span><span class="sxs-lookup"><span data-stu-id="e8d22-139">Relationship</span></span> | <span data-ttu-id="e8d22-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8d22-140">Type</span></span>        | <span data-ttu-id="e8d22-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d22-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8d22-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="e8d22-142">createdBy</span></span>|[<span data-ttu-id="e8d22-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e8d22-143">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="e8d22-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8d22-144">Read-only.</span></span> <span data-ttu-id="e8d22-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e8d22-145">Nullable.</span></span>|
|<span data-ttu-id="e8d22-146">documentos</span><span class="sxs-lookup"><span data-stu-id="e8d22-146">documents</span></span>|<span data-ttu-id="e8d22-147">coleção [AddDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="e8d22-147">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="e8d22-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8d22-148">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8d22-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8d22-149">JSON representation</span></span>

<span data-ttu-id="e8d22-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8d22-150">The following is a JSON representation of the resource.</span></span>

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