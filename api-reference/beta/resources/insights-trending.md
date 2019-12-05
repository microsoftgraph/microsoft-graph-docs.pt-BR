---
title: tipo de recurso de tendência
description: Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário). Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 0b631554cc8cd2ed0c9a76f4c132d36c4b08e0cd
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844306"
---
# <a name="trending-resource-type"></a><span data-ttu-id="61d35-104">tipo de recurso de tendência</span><span class="sxs-lookup"><span data-stu-id="61d35-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61d35-105">Relação avançada conectando um usuário a documentos que estão em tendência ao usuário (são relevantes para o usuário).</span><span class="sxs-lookup"><span data-stu-id="61d35-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="61d35-106">Os arquivos do OneDrive e os arquivos armazenados em sites de equipe do SharePoint podem ser tendências em torno do usuário.</span><span class="sxs-lookup"><span data-stu-id="61d35-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="61d35-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="61d35-107">Methods</span></span>

| <span data-ttu-id="61d35-108">Método</span><span class="sxs-lookup"><span data-stu-id="61d35-108">Method</span></span>       | <span data-ttu-id="61d35-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61d35-109">Return Type</span></span>  |<span data-ttu-id="61d35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d35-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61d35-111">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="61d35-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="61d35-112">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="61d35-112">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="61d35-113">Obtenha uma lista de arquivos de tendência.</span><span class="sxs-lookup"><span data-stu-id="61d35-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="61d35-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61d35-114">Properties</span></span>

| <span data-ttu-id="61d35-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61d35-115">Property</span></span>      | <span data-ttu-id="61d35-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d35-116">Type</span></span>                              | <span data-ttu-id="61d35-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d35-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="61d35-118">id</span><span class="sxs-lookup"><span data-stu-id="61d35-118">id</span></span>                    | <span data-ttu-id="61d35-119">String</span><span class="sxs-lookup"><span data-stu-id="61d35-119">String</span></span>                    | <span data-ttu-id="61d35-120">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="61d35-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="61d35-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61d35-121">Read only.</span></span>        |
| <span data-ttu-id="61d35-122">weight</span><span class="sxs-lookup"><span data-stu-id="61d35-122">weight</span></span>                | <span data-ttu-id="61d35-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="61d35-123">Double</span></span>                    | <span data-ttu-id="61d35-124">Valor que indica quanto o documento está em tendência no momento.</span><span class="sxs-lookup"><span data-stu-id="61d35-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="61d35-125">Quanto maior o número, mais o documento está atualmente em tendência ao usuário (o que é mais relevante).</span><span class="sxs-lookup"><span data-stu-id="61d35-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="61d35-126">Os documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="61d35-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="61d35-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="61d35-127">resourceVisualization</span></span> | [<span data-ttu-id="61d35-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="61d35-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="61d35-129">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="61d35-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="61d35-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="61d35-130">resourceReference</span></span>     | [<span data-ttu-id="61d35-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="61d35-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="61d35-132">Propriedades de referência do documento de tendência, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="61d35-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="61d35-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61d35-133">lastModifiedDateTime</span></span>  | <span data-ttu-id="61d35-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d35-134">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="61d35-135">Relações</span><span class="sxs-lookup"><span data-stu-id="61d35-135">Relationships</span></span>

| <span data-ttu-id="61d35-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61d35-136">Property</span></span>      | <span data-ttu-id="61d35-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="61d35-137">Type</span></span>          | <span data-ttu-id="61d35-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d35-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="61d35-139">recurso</span><span class="sxs-lookup"><span data-stu-id="61d35-139">resource</span></span>      | <span data-ttu-id="61d35-140">entidade</span><span class="sxs-lookup"><span data-stu-id="61d35-140">entity</span></span>        | <span data-ttu-id="61d35-141">Usado para navegar para o documento de tendência.</span><span class="sxs-lookup"><span data-stu-id="61d35-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61d35-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61d35-142">JSON representation</span></span>

<span data-ttu-id="61d35-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="61d35-143">Here is a JSON representation of the resource</span></span>

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
