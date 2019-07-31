---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7963a3c518fd4fc946da4f6714a3aa52aa4b87eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006217"
---
# <a name="trending-resource-type"></a><span data-ttu-id="8091a-104">tipo de recurso de tendência</span><span class="sxs-lookup"><span data-stu-id="8091a-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8091a-105">Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário).</span><span class="sxs-lookup"><span data-stu-id="8091a-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="8091a-106">Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="8091a-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="8091a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8091a-107">Methods</span></span>

| <span data-ttu-id="8091a-108">Método</span><span class="sxs-lookup"><span data-stu-id="8091a-108">Method</span></span>       | <span data-ttu-id="8091a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8091a-109">Return Type</span></span>  |<span data-ttu-id="8091a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8091a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8091a-111">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="8091a-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="8091a-112">coleção [insights_trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="8091a-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="8091a-113">Obtenha uma lista de arquivos de tendência.</span><span class="sxs-lookup"><span data-stu-id="8091a-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="8091a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8091a-114">Properties</span></span>

| <span data-ttu-id="8091a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8091a-115">Property</span></span>      | <span data-ttu-id="8091a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8091a-116">Type</span></span>                              | <span data-ttu-id="8091a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8091a-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="8091a-118">id</span><span class="sxs-lookup"><span data-stu-id="8091a-118">id</span></span>                    | <span data-ttu-id="8091a-119">String</span><span class="sxs-lookup"><span data-stu-id="8091a-119">String</span></span>                    | <span data-ttu-id="8091a-120">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="8091a-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="8091a-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8091a-121">Read only.</span></span>        |
| <span data-ttu-id="8091a-122">weight</span><span class="sxs-lookup"><span data-stu-id="8091a-122">weight</span></span>                | <span data-ttu-id="8091a-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="8091a-123">Double</span></span>                    | <span data-ttu-id="8091a-124">Valor que indica quanto o documento está em tendência no momento.</span><span class="sxs-lookup"><span data-stu-id="8091a-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="8091a-125">Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante).</span><span class="sxs-lookup"><span data-stu-id="8091a-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="8091a-126">Os documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="8091a-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="8091a-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="8091a-127">resourceVisualization</span></span> | [<span data-ttu-id="8091a-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="8091a-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="8091a-129">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="8091a-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="8091a-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="8091a-130">resourceReference</span></span>     | [<span data-ttu-id="8091a-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="8091a-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="8091a-132">Propriedades de referência do documento de tendência, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="8091a-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="8091a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8091a-133">lastModifiedDateTime</span></span>  | <span data-ttu-id="8091a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8091a-134">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="8091a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="8091a-135">Relationships</span></span>

| <span data-ttu-id="8091a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8091a-136">Property</span></span>      | <span data-ttu-id="8091a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8091a-137">Type</span></span>          | <span data-ttu-id="8091a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8091a-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="8091a-139">recurso</span><span class="sxs-lookup"><span data-stu-id="8091a-139">resource</span></span>      | <span data-ttu-id="8091a-140">entidade</span><span class="sxs-lookup"><span data-stu-id="8091a-140">entity</span></span>        | <span data-ttu-id="8091a-141">Usado para navegar para o documento de tendência.</span><span class="sxs-lookup"><span data-stu-id="8091a-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8091a-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8091a-142">JSON representation</span></span>

<span data-ttu-id="8091a-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8091a-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```
