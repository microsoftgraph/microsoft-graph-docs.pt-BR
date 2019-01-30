---
title: tipo de recurso de tendências
description: Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário). Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640368"
---
# <a name="trending-resource-type"></a><span data-ttu-id="32ae9-104">tipo de recurso de tendências</span><span class="sxs-lookup"><span data-stu-id="32ae9-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32ae9-105">Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário).</span><span class="sxs-lookup"><span data-stu-id="32ae9-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="32ae9-106">Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.</span><span class="sxs-lookup"><span data-stu-id="32ae9-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="32ae9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="32ae9-107">Methods</span></span>

| <span data-ttu-id="32ae9-108">Método</span><span class="sxs-lookup"><span data-stu-id="32ae9-108">Method</span></span>       | <span data-ttu-id="32ae9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32ae9-109">Return Type</span></span>  |<span data-ttu-id="32ae9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ae9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32ae9-111">Lista de tendências</span><span class="sxs-lookup"><span data-stu-id="32ae9-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="32ae9-112">coleção [insights_trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="32ae9-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="32ae9-113">Obtenha uma lista dos arquivos de tendências.</span><span class="sxs-lookup"><span data-stu-id="32ae9-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="32ae9-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32ae9-114">Properties</span></span>

| <span data-ttu-id="32ae9-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32ae9-115">Property</span></span>      | <span data-ttu-id="32ae9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="32ae9-116">Type</span></span>                              | <span data-ttu-id="32ae9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ae9-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="32ae9-118">id</span><span class="sxs-lookup"><span data-stu-id="32ae9-118">id</span></span>                    | <span data-ttu-id="32ae9-119">String</span><span class="sxs-lookup"><span data-stu-id="32ae9-119">String</span></span>                    | <span data-ttu-id="32ae9-120">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="32ae9-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="32ae9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="32ae9-121">Read only.</span></span>        |
| <span data-ttu-id="32ae9-122">weight</span><span class="sxs-lookup"><span data-stu-id="32ae9-122">weight</span></span>                | <span data-ttu-id="32ae9-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="32ae9-123">Double</span></span>                    | <span data-ttu-id="32ae9-124">Valor que indica o quanto o documento está atualmente tendências.</span><span class="sxs-lookup"><span data-stu-id="32ae9-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="32ae9-125">Quanto maior o número, mais o documento é atualmente tendências ao redor do usuário (o mais relevantes é).</span><span class="sxs-lookup"><span data-stu-id="32ae9-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="32ae9-126">Documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="32ae9-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="32ae9-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="32ae9-127">resourceVisualization</span></span> | [<span data-ttu-id="32ae9-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="32ae9-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="32ae9-129">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="32ae9-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="32ae9-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="32ae9-130">resourceReference</span></span>     | [<span data-ttu-id="32ae9-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="32ae9-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="32ae9-132">Propriedades de referência do documento tendência, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="32ae9-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="32ae9-133">Relações</span><span class="sxs-lookup"><span data-stu-id="32ae9-133">Relationships</span></span>

| <span data-ttu-id="32ae9-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32ae9-134">Property</span></span>      | <span data-ttu-id="32ae9-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="32ae9-135">Type</span></span>          | <span data-ttu-id="32ae9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="32ae9-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="32ae9-137">recurso</span><span class="sxs-lookup"><span data-stu-id="32ae9-137">resource</span></span>      | <span data-ttu-id="32ae9-138">Entity</span><span class="sxs-lookup"><span data-stu-id="32ae9-138">Entity</span></span>        | <span data-ttu-id="32ae9-139">Usado para navegar até o documento tendência.</span><span class="sxs-lookup"><span data-stu-id="32ae9-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32ae9-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32ae9-140">JSON representation</span></span>

<span data-ttu-id="32ae9-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="32ae9-141">Here is a JSON representation of the resource</span></span>

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
