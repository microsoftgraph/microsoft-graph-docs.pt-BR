---
title: tipo de recurso officeGraphInsights
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 8a07cd10622886ad6e367d5311e750454e7bf90b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348492"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="97813-104">tipo de recurso officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="97813-104">officeGraphInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97813-105">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="97813-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="97813-106">Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.</span><span class="sxs-lookup"><span data-stu-id="97813-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="97813-107">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="97813-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="97813-108">[Tendências](insights-trending.md) – retorna a documentos do OneDrive e de sites do SharePoint de tendências de um usuário à sua volta.</span><span class="sxs-lookup"><span data-stu-id="97813-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="97813-109">[Usado](insights-used.md) - Retornar documentos visualizados e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="97813-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="97813-110">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="97813-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="97813-111">[Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="97813-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="97813-112">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="97813-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="97813-113">Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="97813-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="97813-114">O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="97813-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="97813-115">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="97813-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="97813-116">Relações</span><span class="sxs-lookup"><span data-stu-id="97813-116">Relationships</span></span>

| <span data-ttu-id="97813-117">Relação</span><span class="sxs-lookup"><span data-stu-id="97813-117">Relationship</span></span>      | <span data-ttu-id="97813-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="97813-118">Type</span></span>          | <span data-ttu-id="97813-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97813-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="97813-120">tendências</span><span class="sxs-lookup"><span data-stu-id="97813-120">trending</span></span>      | <span data-ttu-id="97813-121">[tendências](insights-trending.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="97813-121">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="97813-122">Relação calculada identificando documentos mais populares.</span><span class="sxs-lookup"><span data-stu-id="97813-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="97813-123">Os documentos mais populares podem ser armazenados no OneDrive ou em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97813-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="97813-124">usado</span><span class="sxs-lookup"><span data-stu-id="97813-124">used</span></span>      | <span data-ttu-id="97813-125">[usedInsight](insights-used.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="97813-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="97813-126">Relação calculada para identificar documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="97813-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="97813-127">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="97813-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="97813-128">compartilhado</span><span class="sxs-lookup"><span data-stu-id="97813-128">shared</span></span>        | <span data-ttu-id="97813-129">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="97813-129">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="97813-130">Relação calculada identificando documentos mais populares compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="97813-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="97813-131">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="97813-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="97813-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97813-132">JSON representation</span></span>

<span data-ttu-id="97813-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="97813-133">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
