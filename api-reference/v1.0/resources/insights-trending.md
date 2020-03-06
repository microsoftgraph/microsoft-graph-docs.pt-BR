---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a3b836eaf503315b4c47d71fce3f308c35dd8aed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531276"
---
# <a name="trending-resource-type"></a><span data-ttu-id="cceef-104">tipo de recurso de tendência</span><span class="sxs-lookup"><span data-stu-id="cceef-104">trending resource type</span></span>

<span data-ttu-id="cceef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cceef-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cceef-106">Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário).</span><span class="sxs-lookup"><span data-stu-id="cceef-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="cceef-107">Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="cceef-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cceef-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cceef-108">Methods</span></span>

| <span data-ttu-id="cceef-109">Método</span><span class="sxs-lookup"><span data-stu-id="cceef-109">Method</span></span>       | <span data-ttu-id="cceef-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cceef-110">Return Type</span></span>  |<span data-ttu-id="cceef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cceef-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cceef-112">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="cceef-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="cceef-113">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="cceef-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="cceef-114">Obtenha uma lista de arquivos de tendência.</span><span class="sxs-lookup"><span data-stu-id="cceef-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="cceef-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cceef-115">Properties</span></span>

| <span data-ttu-id="cceef-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cceef-116">Property</span></span>      | <span data-ttu-id="cceef-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="cceef-117">Type</span></span>                              | <span data-ttu-id="cceef-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="cceef-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="cceef-119">id</span><span class="sxs-lookup"><span data-stu-id="cceef-119">id</span></span>                    | <span data-ttu-id="cceef-120">String</span><span class="sxs-lookup"><span data-stu-id="cceef-120">String</span></span>                    | <span data-ttu-id="cceef-121">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="cceef-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="cceef-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cceef-122">Read only.</span></span>        |
| <span data-ttu-id="cceef-123">weight</span><span class="sxs-lookup"><span data-stu-id="cceef-123">weight</span></span>                | <span data-ttu-id="cceef-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="cceef-124">Double</span></span>                    | <span data-ttu-id="cceef-125">Valor que indica quanto o documento está em tendência no momento.</span><span class="sxs-lookup"><span data-stu-id="cceef-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="cceef-126">Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante).</span><span class="sxs-lookup"><span data-stu-id="cceef-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="cceef-127">Os documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="cceef-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="cceef-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cceef-128">resourceVisualization</span></span> | [<span data-ttu-id="cceef-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cceef-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="cceef-130">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="cceef-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="cceef-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cceef-131">resourceReference</span></span>     | [<span data-ttu-id="cceef-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cceef-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="cceef-133">Propriedades de referência do documento de tendência, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="cceef-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="cceef-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cceef-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="cceef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cceef-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="cceef-136">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="cceef-136">Relationships</span></span>

| <span data-ttu-id="cceef-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cceef-137">Property</span></span>      | <span data-ttu-id="cceef-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="cceef-138">Type</span></span>          | <span data-ttu-id="cceef-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cceef-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="cceef-140">recurso</span><span class="sxs-lookup"><span data-stu-id="cceef-140">resource</span></span>      | <span data-ttu-id="cceef-141">entidade</span><span class="sxs-lookup"><span data-stu-id="cceef-141">entity</span></span>        | <span data-ttu-id="cceef-142">Usado para navegar para o documento de tendência.</span><span class="sxs-lookup"><span data-stu-id="cceef-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cceef-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cceef-143">JSON representation</span></span>

<span data-ttu-id="cceef-144">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cceef-144">Here is a JSON representation of the resource</span></span>

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
