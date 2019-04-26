---
title: tipo de recurso sharedInsight
description: 'Uma percepção representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 128a85bb9aa2e9f51d2393029cce3c27f8c4e6f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339973"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="67ea8-104">tipo de recurso sharedInsight</span><span class="sxs-lookup"><span data-stu-id="67ea8-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ea8-105">Uma percepção representando arquivos compartilhados com ou por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="67ea8-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="67ea8-106">Há suporte para os seguintes arquivos compartilhados:</span><span class="sxs-lookup"><span data-stu-id="67ea8-106">The following shared files are supported:</span></span>

- <span data-ttu-id="67ea8-107">Arquivos anexados diretamente em um email ou convite de reunião.</span><span class="sxs-lookup"><span data-stu-id="67ea8-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="67ea8-108">OneDrive for bussiness e anexos modernos do SharePoint-arquivos armazenados no OneDrive for Business e SharePoint que os usuários compartilham como links em um email.</span><span class="sxs-lookup"><span data-stu-id="67ea8-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="67ea8-109">**Observação**: no momento, estamos trabalhando para preencher os resultados da API compartilhada com dados.</span><span class="sxs-lookup"><span data-stu-id="67ea8-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="67ea8-110">Pode haver alguns dados ausentes nas primeiras semanas após o lançamento.</span><span class="sxs-lookup"><span data-stu-id="67ea8-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="67ea8-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="67ea8-111">Methods</span></span>

| <span data-ttu-id="67ea8-112">Método</span><span class="sxs-lookup"><span data-stu-id="67ea8-112">Method</span></span>       | <span data-ttu-id="67ea8-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="67ea8-113">Return Type</span></span>  |<span data-ttu-id="67ea8-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ea8-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67ea8-115">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="67ea8-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="67ea8-116">coleção [insights_shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="67ea8-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="67ea8-117">Obter uma lista de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="67ea8-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="67ea8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67ea8-118">Properties</span></span>

| <span data-ttu-id="67ea8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67ea8-119">Property</span></span>              | <span data-ttu-id="67ea8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="67ea8-120">Type</span></span>                      | <span data-ttu-id="67ea8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ea8-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="67ea8-122">id</span><span class="sxs-lookup"><span data-stu-id="67ea8-122">id</span></span>                    | <span data-ttu-id="67ea8-123">String</span><span class="sxs-lookup"><span data-stu-id="67ea8-123">String</span></span>                    | <span data-ttu-id="67ea8-124">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="67ea8-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="67ea8-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67ea8-125">Read only.</span></span>        |
| <span data-ttu-id="67ea8-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="67ea8-126">lastShared</span></span>            | [<span data-ttu-id="67ea8-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="67ea8-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="67ea8-128">Detalhes sobre o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="67ea8-128">Details about the shared item.</span></span> <span data-ttu-id="67ea8-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67ea8-129">Read only.</span></span>        |
| <span data-ttu-id="67ea8-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="67ea8-130">resourceVisualization</span></span> | [<span data-ttu-id="67ea8-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="67ea8-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="67ea8-132">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="67ea8-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="67ea8-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="67ea8-133">Read-only</span></span>      |
| <span data-ttu-id="67ea8-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="67ea8-134">resourceReference</span></span>     | [<span data-ttu-id="67ea8-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="67ea8-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="67ea8-136">Propriedades de referência do documento compartilhado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="67ea8-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="67ea8-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="67ea8-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="67ea8-138">Relações</span><span class="sxs-lookup"><span data-stu-id="67ea8-138">Relationships</span></span>

| <span data-ttu-id="67ea8-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67ea8-139">Property</span></span>      | <span data-ttu-id="67ea8-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="67ea8-140">Type</span></span>          | <span data-ttu-id="67ea8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ea8-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="67ea8-142">recurso</span><span class="sxs-lookup"><span data-stu-id="67ea8-142">resource</span></span>      | <span data-ttu-id="67ea8-143">coleção Entity</span><span class="sxs-lookup"><span data-stu-id="67ea8-143">entity collection</span></span> | <span data-ttu-id="67ea8-144">Usado para navegar até o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="67ea8-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="67ea8-145">Para anexos de arquivo, o tipo \*\* é fileattachment.</span><span class="sxs-lookup"><span data-stu-id="67ea8-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="67ea8-146">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="67ea8-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67ea8-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67ea8-147">JSON representation</span></span>
<span data-ttu-id="67ea8-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="67ea8-148">Here is a JSON representation of the resource</span></span>
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
