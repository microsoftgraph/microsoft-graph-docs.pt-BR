---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a083f612b3cb4808a443938a9b7f1958e8c60a0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986081"
---
# <a name="trending-resource-type"></a><span data-ttu-id="cf7be-104">tipo de recurso de tendência</span><span class="sxs-lookup"><span data-stu-id="cf7be-104">trending resource type</span></span>

<span data-ttu-id="cf7be-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf7be-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf7be-106">Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário).</span><span class="sxs-lookup"><span data-stu-id="cf7be-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="cf7be-107">Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf7be-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cf7be-108">Methods</span><span class="sxs-lookup"><span data-stu-id="cf7be-108">Methods</span></span>

| <span data-ttu-id="cf7be-109">Método</span><span class="sxs-lookup"><span data-stu-id="cf7be-109">Method</span></span>       | <span data-ttu-id="cf7be-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf7be-110">Return Type</span></span>  |<span data-ttu-id="cf7be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf7be-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf7be-112">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="cf7be-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="cf7be-113">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="cf7be-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="cf7be-114">Obtenha uma lista de arquivos de tendência.</span><span class="sxs-lookup"><span data-stu-id="cf7be-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf7be-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf7be-115">Properties</span></span>

| <span data-ttu-id="cf7be-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf7be-116">Property</span></span>      | <span data-ttu-id="cf7be-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf7be-117">Type</span></span>                              | <span data-ttu-id="cf7be-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf7be-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="cf7be-119">id</span><span class="sxs-lookup"><span data-stu-id="cf7be-119">id</span></span>                    | <span data-ttu-id="cf7be-120">String</span><span class="sxs-lookup"><span data-stu-id="cf7be-120">String</span></span>                    | <span data-ttu-id="cf7be-121">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="cf7be-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="cf7be-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf7be-122">Read only.</span></span>        |
| <span data-ttu-id="cf7be-123">weight</span><span class="sxs-lookup"><span data-stu-id="cf7be-123">weight</span></span>                | <span data-ttu-id="cf7be-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="cf7be-124">Double</span></span>                    | <span data-ttu-id="cf7be-125">Valor que indica quanto o documento está em tendência no momento.</span><span class="sxs-lookup"><span data-stu-id="cf7be-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="cf7be-126">Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante).</span><span class="sxs-lookup"><span data-stu-id="cf7be-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="cf7be-127">Os documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="cf7be-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="cf7be-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cf7be-128">resourceVisualization</span></span> | [<span data-ttu-id="cf7be-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cf7be-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="cf7be-130">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="cf7be-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="cf7be-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cf7be-131">resourceReference</span></span>     | [<span data-ttu-id="cf7be-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cf7be-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="cf7be-133">Propriedades de referência do documento de tendência, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="cf7be-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="cf7be-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf7be-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="cf7be-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf7be-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="cf7be-136">Relações</span><span class="sxs-lookup"><span data-stu-id="cf7be-136">Relationships</span></span>

| <span data-ttu-id="cf7be-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf7be-137">Property</span></span>      | <span data-ttu-id="cf7be-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf7be-138">Type</span></span>          | <span data-ttu-id="cf7be-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf7be-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="cf7be-140">recurso</span><span class="sxs-lookup"><span data-stu-id="cf7be-140">resource</span></span>      | <span data-ttu-id="cf7be-141">entidade</span><span class="sxs-lookup"><span data-stu-id="cf7be-141">entity</span></span>        | <span data-ttu-id="cf7be-142">Usado para navegar para o documento de tendência.</span><span class="sxs-lookup"><span data-stu-id="cf7be-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf7be-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf7be-143">JSON representation</span></span>

<span data-ttu-id="cf7be-144">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cf7be-144">Here is a JSON representation of the resource</span></span>

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


