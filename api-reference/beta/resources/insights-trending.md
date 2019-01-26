---
title: tipo de recurso de tendências
description: Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário). Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 587b52107f3a7f9892603afb8273ce55b6faa549
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577407"
---
# <a name="trending-resource-type"></a><span data-ttu-id="56164-104">tipo de recurso de tendências</span><span class="sxs-lookup"><span data-stu-id="56164-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56164-105">Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário).</span><span class="sxs-lookup"><span data-stu-id="56164-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="56164-106">Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.</span><span class="sxs-lookup"><span data-stu-id="56164-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="56164-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="56164-107">Methods</span></span>

| <span data-ttu-id="56164-108">Método</span><span class="sxs-lookup"><span data-stu-id="56164-108">Method</span></span>       | <span data-ttu-id="56164-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56164-109">Return Type</span></span>  |<span data-ttu-id="56164-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56164-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56164-111">Lista de tendências</span><span class="sxs-lookup"><span data-stu-id="56164-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="56164-112">coleção [insights_trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="56164-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="56164-113">Obtenha uma lista dos arquivos de tendências.</span><span class="sxs-lookup"><span data-stu-id="56164-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="56164-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56164-114">Properties</span></span>

| <span data-ttu-id="56164-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56164-115">Property</span></span>      | <span data-ttu-id="56164-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="56164-116">Type</span></span>                              | <span data-ttu-id="56164-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="56164-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="56164-118">id</span><span class="sxs-lookup"><span data-stu-id="56164-118">id</span></span>                    | <span data-ttu-id="56164-119">String</span><span class="sxs-lookup"><span data-stu-id="56164-119">String</span></span>                    | <span data-ttu-id="56164-120">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="56164-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="56164-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56164-121">Read only.</span></span>        |
| <span data-ttu-id="56164-122">weight</span><span class="sxs-lookup"><span data-stu-id="56164-122">weight</span></span>                | <span data-ttu-id="56164-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="56164-123">Double</span></span>                    | <span data-ttu-id="56164-124">Valor que indica o quanto o documento está atualmente tendências.</span><span class="sxs-lookup"><span data-stu-id="56164-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="56164-125">Quanto maior o número, mais o documento é atualmente tendências ao redor do usuário (o mais relevantes é).</span><span class="sxs-lookup"><span data-stu-id="56164-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="56164-126">Documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="56164-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="56164-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="56164-127">resourceVisualization</span></span> | <span data-ttu-id="56164-128">coleção [resourceVisualization](insights-resourcevisualization.md)</span><span class="sxs-lookup"><span data-stu-id="56164-128">[resourceVisualization](insights-resourcevisualization.md) collection</span></span> | <span data-ttu-id="56164-129">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="56164-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="56164-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="56164-130">resourceReference</span></span>     | <span data-ttu-id="56164-131">coleção [resourceReference](insights-resourcereference.md)</span><span class="sxs-lookup"><span data-stu-id="56164-131">[resourceReference](insights-resourcereference.md) collection</span></span> | <span data-ttu-id="56164-132">Propriedades de referência do documento tendência, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="56164-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="56164-133">Relações</span><span class="sxs-lookup"><span data-stu-id="56164-133">Relationships</span></span>

| <span data-ttu-id="56164-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56164-134">Property</span></span>      | <span data-ttu-id="56164-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="56164-135">Type</span></span>          | <span data-ttu-id="56164-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="56164-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="56164-137">recurso</span><span class="sxs-lookup"><span data-stu-id="56164-137">resource</span></span>      | <span data-ttu-id="56164-138">coleção de entidade</span><span class="sxs-lookup"><span data-stu-id="56164-138">entity collection</span></span> | <span data-ttu-id="56164-139">Usado para navegar até o documento tendência.</span><span class="sxs-lookup"><span data-stu-id="56164-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56164-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56164-140">JSON representation</span></span>

<span data-ttu-id="56164-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="56164-141">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trending"
}-->
```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
