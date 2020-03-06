---
title: tipo de recurso sharedInsight
description: 'Uma percepção representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b7bb8c2a69ebab16171ff4a74283d0993aefc8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532874"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="f0aee-104">tipo de recurso sharedInsight</span><span class="sxs-lookup"><span data-stu-id="f0aee-104">sharedInsight resource type</span></span>

<span data-ttu-id="f0aee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0aee-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0aee-106">Uma percepção representando arquivos compartilhados com ou por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="f0aee-106">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="f0aee-107">Há suporte para os seguintes arquivos compartilhados:</span><span class="sxs-lookup"><span data-stu-id="f0aee-107">The following shared files are supported:</span></span>

- <span data-ttu-id="f0aee-108">Arquivos anexados diretamente em um email ou convite de reunião.</span><span class="sxs-lookup"><span data-stu-id="f0aee-108">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="f0aee-109">O OneDrive for Business e o SharePoint Modern Attachments-arquivos armazenados no OneDrive for Business e no SharePoint que os usuários compartilham como links em um email.</span><span class="sxs-lookup"><span data-stu-id="f0aee-109">OneDrive for Business and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="f0aee-110">**Observação**: no momento, estamos trabalhando para preencher os resultados da API compartilhada com dados.</span><span class="sxs-lookup"><span data-stu-id="f0aee-110">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="f0aee-111">Pode haver alguns dados ausentes nas primeiras semanas após o lançamento.</span><span class="sxs-lookup"><span data-stu-id="f0aee-111">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="f0aee-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0aee-112">Methods</span></span>

| <span data-ttu-id="f0aee-113">Método</span><span class="sxs-lookup"><span data-stu-id="f0aee-113">Method</span></span>       | <span data-ttu-id="f0aee-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0aee-114">Return Type</span></span>  |<span data-ttu-id="f0aee-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aee-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0aee-116">Listar compartilhado</span><span class="sxs-lookup"><span data-stu-id="f0aee-116">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="f0aee-117">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="f0aee-117">[sharedInsight](insights-shared.md) collection</span></span>| <span data-ttu-id="f0aee-118">Obter uma lista de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="f0aee-118">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0aee-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0aee-119">Properties</span></span>

| <span data-ttu-id="f0aee-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0aee-120">Property</span></span>              | <span data-ttu-id="f0aee-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aee-121">Type</span></span>                      | <span data-ttu-id="f0aee-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aee-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="f0aee-123">id</span><span class="sxs-lookup"><span data-stu-id="f0aee-123">id</span></span>                    | <span data-ttu-id="f0aee-124">String</span><span class="sxs-lookup"><span data-stu-id="f0aee-124">String</span></span>                    | <span data-ttu-id="f0aee-125">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="f0aee-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="f0aee-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0aee-126">Read only.</span></span>        |
| <span data-ttu-id="f0aee-127">lastShared</span><span class="sxs-lookup"><span data-stu-id="f0aee-127">lastShared</span></span>            | [<span data-ttu-id="f0aee-128">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="f0aee-128">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="f0aee-129">Detalhes sobre o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f0aee-129">Details about the shared item.</span></span> <span data-ttu-id="f0aee-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0aee-130">Read only.</span></span>        |
| <span data-ttu-id="f0aee-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f0aee-131">resourceVisualization</span></span> | [<span data-ttu-id="f0aee-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f0aee-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="f0aee-133">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="f0aee-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="f0aee-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f0aee-134">Read-only</span></span>      |
| <span data-ttu-id="f0aee-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f0aee-135">resourceReference</span></span>     | [<span data-ttu-id="f0aee-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f0aee-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="f0aee-137">Propriedades de referência do documento compartilhado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="f0aee-137">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="f0aee-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="f0aee-138">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="f0aee-139">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="f0aee-139">Relationships</span></span>

| <span data-ttu-id="f0aee-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0aee-140">Property</span></span>      | <span data-ttu-id="f0aee-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aee-141">Type</span></span>          | <span data-ttu-id="f0aee-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aee-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="f0aee-143">recurso</span><span class="sxs-lookup"><span data-stu-id="f0aee-143">resource</span></span>      | <span data-ttu-id="f0aee-144">coleção Entity</span><span class="sxs-lookup"><span data-stu-id="f0aee-144">entity collection</span></span> | <span data-ttu-id="f0aee-145">Usado para navegar até o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f0aee-145">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="f0aee-146">Para anexos de arquivo, o tipo é *Fileattachment*.</span><span class="sxs-lookup"><span data-stu-id="f0aee-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="f0aee-147">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="f0aee-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0aee-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0aee-148">JSON representation</span></span>
<span data-ttu-id="f0aee-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f0aee-149">Here is a JSON representation of the resource</span></span>
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
