---
title: usado o tipo de recurso
description: Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525854"
---
# <a name="used-resource-type"></a><span data-ttu-id="1501e-104">usado o tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="1501e-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1501e-105">Uma compreensão dos representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="1501e-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="1501e-106">As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.</span><span class="sxs-lookup"><span data-stu-id="1501e-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="1501e-107">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="1501e-107">This includes documents in:</span></span>

- <span data-ttu-id="1501e-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="1501e-108">OneDrive for Business</span></span>
- <span data-ttu-id="1501e-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="1501e-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="1501e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="1501e-110">Methods</span></span>

| <span data-ttu-id="1501e-111">Método</span><span class="sxs-lookup"><span data-stu-id="1501e-111">Method</span></span>       | <span data-ttu-id="1501e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1501e-112">Return Type</span></span>  |<span data-ttu-id="1501e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1501e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1501e-114">Lista usada</span><span class="sxs-lookup"><span data-stu-id="1501e-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="1501e-115">coleção [insights_used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="1501e-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="1501e-116">Obtenha uma lista de arquivos utilizados.</span><span class="sxs-lookup"><span data-stu-id="1501e-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="1501e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1501e-117">Properties</span></span>

| <span data-ttu-id="1501e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1501e-118">Property</span></span>              | <span data-ttu-id="1501e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1501e-119">Type</span></span>                      | <span data-ttu-id="1501e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1501e-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="1501e-121">id</span><span class="sxs-lookup"><span data-stu-id="1501e-121">id</span></span>                    | <span data-ttu-id="1501e-122">String</span><span class="sxs-lookup"><span data-stu-id="1501e-122">String</span></span>                    | <span data-ttu-id="1501e-123">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="1501e-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="1501e-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1501e-124">Read only.</span></span>        |
| <span data-ttu-id="1501e-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="1501e-125">lastUsed</span></span>              | [<span data-ttu-id="1501e-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="1501e-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="1501e-127">Informações sobre quando o item foi último exibidos e modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1501e-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="1501e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1501e-128">Read only.</span></span>     |
| <span data-ttu-id="1501e-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1501e-129">resourceVisualization</span></span> | [<span data-ttu-id="1501e-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1501e-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="1501e-131">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="1501e-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="1501e-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1501e-132">Read-only</span></span>      |
| <span data-ttu-id="1501e-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1501e-133">resourceReference</span></span>     | [<span data-ttu-id="1501e-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1501e-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="1501e-135">Propriedades de referência do documento usado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="1501e-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="1501e-136">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1501e-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="1501e-137">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1501e-137">Relationships</span></span>

| <span data-ttu-id="1501e-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1501e-138">Property</span></span>      | <span data-ttu-id="1501e-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="1501e-139">Type</span></span>          | <span data-ttu-id="1501e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="1501e-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="1501e-141">recurso</span><span class="sxs-lookup"><span data-stu-id="1501e-141">resource</span></span>      | <span data-ttu-id="1501e-142">Entity</span><span class="sxs-lookup"><span data-stu-id="1501e-142">Entity</span></span>        | <span data-ttu-id="1501e-143">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="1501e-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="1501e-144">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="1501e-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="1501e-145">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="1501e-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1501e-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1501e-146">JSON representation</span></span>
<span data-ttu-id="1501e-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1501e-147">Here is a JSON representation of the resource</span></span>

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
