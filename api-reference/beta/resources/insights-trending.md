---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551306"
---
# <a name="trending-resource-type"></a><span data-ttu-id="9655f-104">tipo de recurso de tendência</span><span class="sxs-lookup"><span data-stu-id="9655f-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9655f-105">Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário).</span><span class="sxs-lookup"><span data-stu-id="9655f-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="9655f-106">Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="9655f-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="9655f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9655f-107">Methods</span></span>

| <span data-ttu-id="9655f-108">Método</span><span class="sxs-lookup"><span data-stu-id="9655f-108">Method</span></span>       | <span data-ttu-id="9655f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9655f-109">Return Type</span></span>  |<span data-ttu-id="9655f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9655f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9655f-111">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="9655f-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="9655f-112">coleção [insights_trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="9655f-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="9655f-113">Obtenha uma lista de arquivos de tendência.</span><span class="sxs-lookup"><span data-stu-id="9655f-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="9655f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9655f-114">Properties</span></span>

| <span data-ttu-id="9655f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9655f-115">Property</span></span>      | <span data-ttu-id="9655f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="9655f-116">Type</span></span>                              | <span data-ttu-id="9655f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9655f-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="9655f-118">id</span><span class="sxs-lookup"><span data-stu-id="9655f-118">id</span></span>                    | <span data-ttu-id="9655f-119">String</span><span class="sxs-lookup"><span data-stu-id="9655f-119">String</span></span>                    | <span data-ttu-id="9655f-120">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="9655f-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="9655f-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9655f-121">Read only.</span></span>        |
| <span data-ttu-id="9655f-122">weight</span><span class="sxs-lookup"><span data-stu-id="9655f-122">weight</span></span>                | <span data-ttu-id="9655f-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="9655f-123">Double</span></span>                    | <span data-ttu-id="9655f-124">Valor que indica quanto o documento está em tendência no momento.</span><span class="sxs-lookup"><span data-stu-id="9655f-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="9655f-125">Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante).</span><span class="sxs-lookup"><span data-stu-id="9655f-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="9655f-126">Os documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="9655f-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="9655f-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="9655f-127">resourceVisualization</span></span> | [<span data-ttu-id="9655f-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="9655f-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="9655f-129">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="9655f-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="9655f-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="9655f-130">resourceReference</span></span>     | [<span data-ttu-id="9655f-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="9655f-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="9655f-132">Propriedades de referência do documento de tendência, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="9655f-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9655f-133">Relações</span><span class="sxs-lookup"><span data-stu-id="9655f-133">Relationships</span></span>

| <span data-ttu-id="9655f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9655f-134">Property</span></span>      | <span data-ttu-id="9655f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="9655f-135">Type</span></span>          | <span data-ttu-id="9655f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="9655f-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="9655f-137">recurso</span><span class="sxs-lookup"><span data-stu-id="9655f-137">resource</span></span>      | <span data-ttu-id="9655f-138">Entidade</span><span class="sxs-lookup"><span data-stu-id="9655f-138">Entity</span></span>        | <span data-ttu-id="9655f-139">Usado para navegar para o documento de tendência.</span><span class="sxs-lookup"><span data-stu-id="9655f-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9655f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9655f-140">JSON representation</span></span>

<span data-ttu-id="9655f-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9655f-141">Here is a JSON representation of the resource</span></span>

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
