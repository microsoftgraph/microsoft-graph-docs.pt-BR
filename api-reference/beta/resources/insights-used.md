---
title: tipo de recurso usado
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551285"
---
# <a name="used-resource-type"></a><span data-ttu-id="3da4c-104">tipo de recurso usado</span><span class="sxs-lookup"><span data-stu-id="3da4c-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da4c-105">Uma percepção representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="3da4c-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="3da4c-106">O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.</span><span class="sxs-lookup"><span data-stu-id="3da4c-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="3da4c-107">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="3da4c-107">This includes documents in:</span></span>

- <span data-ttu-id="3da4c-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="3da4c-108">OneDrive for Business</span></span>
- <span data-ttu-id="3da4c-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="3da4c-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="3da4c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="3da4c-110">Methods</span></span>

| <span data-ttu-id="3da4c-111">Método</span><span class="sxs-lookup"><span data-stu-id="3da4c-111">Method</span></span>       | <span data-ttu-id="3da4c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3da4c-112">Return Type</span></span>  |<span data-ttu-id="3da4c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da4c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3da4c-114">Listar usados</span><span class="sxs-lookup"><span data-stu-id="3da4c-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="3da4c-115">coleção [insights_used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="3da4c-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="3da4c-116">Obtenha uma lista de arquivos usados.</span><span class="sxs-lookup"><span data-stu-id="3da4c-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="3da4c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3da4c-117">Properties</span></span>

| <span data-ttu-id="3da4c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3da4c-118">Property</span></span>              | <span data-ttu-id="3da4c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3da4c-119">Type</span></span>                      | <span data-ttu-id="3da4c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da4c-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="3da4c-121">id</span><span class="sxs-lookup"><span data-stu-id="3da4c-121">id</span></span>                    | <span data-ttu-id="3da4c-122">String</span><span class="sxs-lookup"><span data-stu-id="3da4c-122">String</span></span>                    | <span data-ttu-id="3da4c-123">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="3da4c-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="3da4c-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3da4c-124">Read only.</span></span>        |
| <span data-ttu-id="3da4c-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="3da4c-125">lastUsed</span></span>              | [<span data-ttu-id="3da4c-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="3da4c-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="3da4c-127">Informações sobre quando o item foi exibido e modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3da4c-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="3da4c-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3da4c-128">Read only.</span></span>     |
| <span data-ttu-id="3da4c-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="3da4c-129">resourceVisualization</span></span> | [<span data-ttu-id="3da4c-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="3da4c-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="3da4c-131">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="3da4c-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="3da4c-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="3da4c-132">Read-only</span></span>      |
| <span data-ttu-id="3da4c-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="3da4c-133">resourceReference</span></span>     | [<span data-ttu-id="3da4c-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="3da4c-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="3da4c-135">Propriedades de referência do documento usado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="3da4c-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="3da4c-136">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="3da4c-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="3da4c-137">Relações</span><span class="sxs-lookup"><span data-stu-id="3da4c-137">Relationships</span></span>

| <span data-ttu-id="3da4c-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3da4c-138">Property</span></span>      | <span data-ttu-id="3da4c-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="3da4c-139">Type</span></span>          | <span data-ttu-id="3da4c-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da4c-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="3da4c-141">recurso</span><span class="sxs-lookup"><span data-stu-id="3da4c-141">resource</span></span>      | <span data-ttu-id="3da4c-142">Entidade</span><span class="sxs-lookup"><span data-stu-id="3da4c-142">Entity</span></span>        | <span data-ttu-id="3da4c-143">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="3da4c-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="3da4c-144">Para anexos de arquivo, o tipo \*\* é fileattachment.</span><span class="sxs-lookup"><span data-stu-id="3da4c-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="3da4c-145">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="3da4c-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3da4c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3da4c-146">JSON representation</span></span>
<span data-ttu-id="3da4c-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3da4c-147">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
