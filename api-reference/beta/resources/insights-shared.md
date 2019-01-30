---
title: tipo de recurso compartilhado
description: 'Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640123"
---
# <a name="shared-resource-type"></a><span data-ttu-id="18d08-104">tipo de recurso compartilhado</span><span class="sxs-lookup"><span data-stu-id="18d08-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d08-105">Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="18d08-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="18d08-106">Há suporte para os seguintes arquivos compartilhados:</span><span class="sxs-lookup"><span data-stu-id="18d08-106">The following shared files are supported:</span></span>

- <span data-ttu-id="18d08-107">Arquivos anexados diretamente em um email ou uma reunião convidem.</span><span class="sxs-lookup"><span data-stu-id="18d08-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="18d08-108">OneDrive para Bussiness e SharePoint modernos anexos - arquivos armazenados no OneDrive para negócios e do SharePoint que os usuários compartilhem como links em um email.</span><span class="sxs-lookup"><span data-stu-id="18d08-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="18d08-109">**Observação**: estamos atualmente trabalhando em preencher os resultados da API compartilhados com dados.</span><span class="sxs-lookup"><span data-stu-id="18d08-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="18d08-110">Pode haver alguns dados ausentes nas semanas primeira depois do lançamento.</span><span class="sxs-lookup"><span data-stu-id="18d08-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="18d08-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="18d08-111">Methods</span></span>

| <span data-ttu-id="18d08-112">Método</span><span class="sxs-lookup"><span data-stu-id="18d08-112">Method</span></span>       | <span data-ttu-id="18d08-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18d08-113">Return Type</span></span>  |<span data-ttu-id="18d08-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d08-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18d08-115">Lista compartilhada</span><span class="sxs-lookup"><span data-stu-id="18d08-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="18d08-116">coleção [insights_shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="18d08-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="18d08-117">Obtenha uma lista de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="18d08-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="18d08-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18d08-118">Properties</span></span>

| <span data-ttu-id="18d08-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d08-119">Property</span></span>              | <span data-ttu-id="18d08-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d08-120">Type</span></span>                      | <span data-ttu-id="18d08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d08-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="18d08-122">id</span><span class="sxs-lookup"><span data-stu-id="18d08-122">id</span></span>                    | <span data-ttu-id="18d08-123">String</span><span class="sxs-lookup"><span data-stu-id="18d08-123">String</span></span>                    | <span data-ttu-id="18d08-124">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="18d08-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="18d08-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18d08-125">Read only.</span></span>        |
| <span data-ttu-id="18d08-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="18d08-126">lastShared</span></span>            | [<span data-ttu-id="18d08-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="18d08-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="18d08-128">Detalhes sobre o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="18d08-128">Details about the shared item.</span></span> <span data-ttu-id="18d08-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18d08-129">Read only.</span></span>        |
| <span data-ttu-id="18d08-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="18d08-130">resourceVisualization</span></span> | [<span data-ttu-id="18d08-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="18d08-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="18d08-132">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="18d08-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="18d08-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="18d08-133">Read-only</span></span>      |
| <span data-ttu-id="18d08-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="18d08-134">resourceReference</span></span>     | [<span data-ttu-id="18d08-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="18d08-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="18d08-136">Propriedades de referência do documento compartilhado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="18d08-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="18d08-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="18d08-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="18d08-138">Relações</span><span class="sxs-lookup"><span data-stu-id="18d08-138">Relationships</span></span>

| <span data-ttu-id="18d08-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d08-139">Property</span></span>      | <span data-ttu-id="18d08-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d08-140">Type</span></span>          | <span data-ttu-id="18d08-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d08-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="18d08-142">recurso</span><span class="sxs-lookup"><span data-stu-id="18d08-142">resource</span></span>      | <span data-ttu-id="18d08-143">Entity</span><span class="sxs-lookup"><span data-stu-id="18d08-143">Entity</span></span>        | <span data-ttu-id="18d08-144">Usado para navegar até o item que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="18d08-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="18d08-145">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="18d08-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="18d08-146">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="18d08-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18d08-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18d08-147">JSON representation</span></span>
<span data-ttu-id="18d08-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="18d08-148">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
