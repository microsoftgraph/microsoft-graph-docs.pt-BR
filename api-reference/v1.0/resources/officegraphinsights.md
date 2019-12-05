---
title: tipo de recurso officeGraphInsights
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1ef2aa97cf9ba5d834a44fc5f338ff933330f491
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844201"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="e0e46-104">tipo de recurso officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="e0e46-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="e0e46-105">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="e0e46-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="e0e46-106">Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.</span><span class="sxs-lookup"><span data-stu-id="e0e46-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="e0e46-107">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="e0e46-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="e0e46-108">[Tendências](insights-trending.md) – retorna a documentos do OneDrive e de sites do SharePoint de tendências de um usuário à sua volta.</span><span class="sxs-lookup"><span data-stu-id="e0e46-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="e0e46-109">[Usado](insights-used.md) - Retornar documentos visualizados e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0e46-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="e0e46-110">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="e0e46-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="e0e46-111">[Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0e46-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="e0e46-112">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="e0e46-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="e0e46-113">Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="e0e46-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="e0e46-114">O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="e0e46-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="e0e46-115">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="e0e46-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="e0e46-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e0e46-116">Relationships</span></span>

| <span data-ttu-id="e0e46-117">Relação</span><span class="sxs-lookup"><span data-stu-id="e0e46-117">Relationship</span></span>      | <span data-ttu-id="e0e46-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0e46-118">Type</span></span>          | <span data-ttu-id="e0e46-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e46-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="e0e46-120">tendências</span><span class="sxs-lookup"><span data-stu-id="e0e46-120">trending</span></span>      | <span data-ttu-id="e0e46-121">[tendências](insights-trending.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="e0e46-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="e0e46-122">Relação calculada identificando documentos mais populares.</span><span class="sxs-lookup"><span data-stu-id="e0e46-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="e0e46-123">Os documentos mais populares podem ser armazenados no OneDrive ou em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e0e46-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="e0e46-124">usado</span><span class="sxs-lookup"><span data-stu-id="e0e46-124">used</span></span>      | <span data-ttu-id="e0e46-125">[usedInsight](insights-used.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="e0e46-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="e0e46-126">Relação calculada para identificar documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0e46-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="e0e46-127">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="e0e46-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="e0e46-128">compartilhado</span><span class="sxs-lookup"><span data-stu-id="e0e46-128">shared</span></span>        | <span data-ttu-id="e0e46-129">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="e0e46-129">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="e0e46-130">Relação calculada identificando documentos mais populares compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0e46-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="e0e46-131">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="e0e46-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="e0e46-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0e46-132">JSON representation</span></span>

<span data-ttu-id="e0e46-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e0e46-133">Here is a JSON representation of the resource</span></span>
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
