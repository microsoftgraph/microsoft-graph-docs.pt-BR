---
title: tipo de recurso sharedInsight
description: 'Uma percepção representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c0af37fb5915fa3d1ec69feecc9bcbf472b4a85a
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844215"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="81e0b-104">tipo de recurso sharedInsight</span><span class="sxs-lookup"><span data-stu-id="81e0b-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81e0b-105">Uma percepção representando arquivos compartilhados com ou por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="81e0b-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="81e0b-106">Há suporte para os seguintes arquivos compartilhados:</span><span class="sxs-lookup"><span data-stu-id="81e0b-106">The following shared files are supported:</span></span>

- <span data-ttu-id="81e0b-107">Arquivos anexados diretamente em um email ou convite de reunião.</span><span class="sxs-lookup"><span data-stu-id="81e0b-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="81e0b-108">O OneDrive for Business e o SharePoint Modern Attachments-arquivos armazenados no OneDrive for Business e no SharePoint que os usuários compartilham como links em um email.</span><span class="sxs-lookup"><span data-stu-id="81e0b-108">OneDrive for Business and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="81e0b-109">**Observação**: no momento, estamos trabalhando para preencher os resultados da API compartilhada com dados.</span><span class="sxs-lookup"><span data-stu-id="81e0b-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="81e0b-110">Pode haver alguns dados ausentes nas primeiras semanas após o lançamento.</span><span class="sxs-lookup"><span data-stu-id="81e0b-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="81e0b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="81e0b-111">Methods</span></span>

| <span data-ttu-id="81e0b-112">Método</span><span class="sxs-lookup"><span data-stu-id="81e0b-112">Method</span></span>       | <span data-ttu-id="81e0b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81e0b-113">Return Type</span></span>  |<span data-ttu-id="81e0b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="81e0b-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81e0b-115">Listar compartilhado</span><span class="sxs-lookup"><span data-stu-id="81e0b-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="81e0b-116">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="81e0b-116">[sharedInsight](insights-shared.md) collection</span></span>| <span data-ttu-id="81e0b-117">Obter uma lista de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="81e0b-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e0b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81e0b-118">Properties</span></span>

| <span data-ttu-id="81e0b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81e0b-119">Property</span></span>              | <span data-ttu-id="81e0b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="81e0b-120">Type</span></span>                      | <span data-ttu-id="81e0b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="81e0b-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="81e0b-122">id</span><span class="sxs-lookup"><span data-stu-id="81e0b-122">id</span></span>                    | <span data-ttu-id="81e0b-123">String</span><span class="sxs-lookup"><span data-stu-id="81e0b-123">String</span></span>                    | <span data-ttu-id="81e0b-124">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="81e0b-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="81e0b-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81e0b-125">Read only.</span></span>        |
| <span data-ttu-id="81e0b-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="81e0b-126">lastShared</span></span>            | [<span data-ttu-id="81e0b-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="81e0b-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="81e0b-128">Detalhes sobre o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="81e0b-128">Details about the shared item.</span></span> <span data-ttu-id="81e0b-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81e0b-129">Read only.</span></span>        |
| <span data-ttu-id="81e0b-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="81e0b-130">resourceVisualization</span></span> | [<span data-ttu-id="81e0b-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="81e0b-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="81e0b-132">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="81e0b-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="81e0b-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="81e0b-133">Read-only</span></span>      |
| <span data-ttu-id="81e0b-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="81e0b-134">resourceReference</span></span>     | [<span data-ttu-id="81e0b-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="81e0b-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="81e0b-136">Propriedades de referência do documento compartilhado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="81e0b-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="81e0b-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="81e0b-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="81e0b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="81e0b-138">Relationships</span></span>

| <span data-ttu-id="81e0b-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81e0b-139">Property</span></span>      | <span data-ttu-id="81e0b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="81e0b-140">Type</span></span>          | <span data-ttu-id="81e0b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="81e0b-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="81e0b-142">recurso</span><span class="sxs-lookup"><span data-stu-id="81e0b-142">resource</span></span>      | <span data-ttu-id="81e0b-143">coleção Entity</span><span class="sxs-lookup"><span data-stu-id="81e0b-143">entity collection</span></span> | <span data-ttu-id="81e0b-144">Usado para navegar até o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="81e0b-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="81e0b-145">Para anexos de arquivo, o tipo é *Fileattachment*.</span><span class="sxs-lookup"><span data-stu-id="81e0b-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="81e0b-146">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="81e0b-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81e0b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81e0b-147">JSON representation</span></span>
<span data-ttu-id="81e0b-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="81e0b-148">Here is a JSON representation of the resource</span></span>
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
