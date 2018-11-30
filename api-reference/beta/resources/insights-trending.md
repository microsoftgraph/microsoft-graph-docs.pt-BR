---
title: tipo de recurso de tendências
description: Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário). Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.
ms.openlocfilehash: 7d240c4358047ca9ba3d6b8340fbfb7d893a6a1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037159"
---
# <a name="trending-resource-type"></a><span data-ttu-id="68aa6-104">tipo de recurso de tendências</span><span class="sxs-lookup"><span data-stu-id="68aa6-104">trending resource type</span></span>

> <span data-ttu-id="68aa6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="68aa6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68aa6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68aa6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68aa6-107">Relacionamento de rich conectando a um usuário a documentos que são tendências em torno do usuário (são relevante para o usuário).</span><span class="sxs-lookup"><span data-stu-id="68aa6-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="68aa6-108">Arquivos de OneDrive, os arquivos armazenados em sites de equipe do SharePoint podem tendências em torno do usuário e.</span><span class="sxs-lookup"><span data-stu-id="68aa6-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="68aa6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="68aa6-109">Methods</span></span>

| <span data-ttu-id="68aa6-110">Método</span><span class="sxs-lookup"><span data-stu-id="68aa6-110">Method</span></span>       | <span data-ttu-id="68aa6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68aa6-111">Return Type</span></span>  |<span data-ttu-id="68aa6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="68aa6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68aa6-113">Lista de tendências</span><span class="sxs-lookup"><span data-stu-id="68aa6-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="68aa6-114">coleção [insights_trending](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="68aa6-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="68aa6-115">Obtenha uma lista dos arquivos de tendências.</span><span class="sxs-lookup"><span data-stu-id="68aa6-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="68aa6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68aa6-116">Properties</span></span>

| <span data-ttu-id="68aa6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68aa6-117">Property</span></span>      | <span data-ttu-id="68aa6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="68aa6-118">Type</span></span>                              | <span data-ttu-id="68aa6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="68aa6-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="68aa6-120">id</span><span class="sxs-lookup"><span data-stu-id="68aa6-120">id</span></span>                    | <span data-ttu-id="68aa6-121">String</span><span class="sxs-lookup"><span data-stu-id="68aa6-121">String</span></span>                    | <span data-ttu-id="68aa6-122">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="68aa6-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="68aa6-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68aa6-123">Read only.</span></span>        |
| <span data-ttu-id="68aa6-124">weight</span><span class="sxs-lookup"><span data-stu-id="68aa6-124">weight</span></span>                | <span data-ttu-id="68aa6-125">Duplo</span><span class="sxs-lookup"><span data-stu-id="68aa6-125">Double</span></span>                    | <span data-ttu-id="68aa6-126">Valor que indica o quanto o documento está atualmente tendências.</span><span class="sxs-lookup"><span data-stu-id="68aa6-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="68aa6-127">Quanto maior o número, mais o documento é atualmente tendências ao redor do usuário (o mais relevantes é).</span><span class="sxs-lookup"><span data-stu-id="68aa6-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="68aa6-128">Documentos retornados são classificados por esse valor.</span><span class="sxs-lookup"><span data-stu-id="68aa6-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="68aa6-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="68aa6-129">resourceVisualization</span></span> | [<span data-ttu-id="68aa6-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="68aa6-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="68aa6-131">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="68aa6-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="68aa6-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="68aa6-132">resourceReference</span></span>     | [<span data-ttu-id="68aa6-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="68aa6-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="68aa6-134">Propriedades de referência do documento tendência, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="68aa6-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="68aa6-135">Relações</span><span class="sxs-lookup"><span data-stu-id="68aa6-135">Relationships</span></span>

| <span data-ttu-id="68aa6-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68aa6-136">Property</span></span>      | <span data-ttu-id="68aa6-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="68aa6-137">Type</span></span>          | <span data-ttu-id="68aa6-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="68aa6-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="68aa6-139">recurso</span><span class="sxs-lookup"><span data-stu-id="68aa6-139">resource</span></span>      | <span data-ttu-id="68aa6-140">Entidade</span><span class="sxs-lookup"><span data-stu-id="68aa6-140">Entity</span></span>        | <span data-ttu-id="68aa6-141">Usado para navegar até o documento tendência.</span><span class="sxs-lookup"><span data-stu-id="68aa6-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68aa6-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68aa6-142">JSON representation</span></span>

<span data-ttu-id="68aa6-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="68aa6-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```