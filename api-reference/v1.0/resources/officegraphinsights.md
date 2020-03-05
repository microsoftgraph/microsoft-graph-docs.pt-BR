---
title: tipo de recurso officeGraphInsights
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8ac5019909a2f5ebe808be695ed7d516738c21e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447336"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="568ee-104">tipo de recurso officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="568ee-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="568ee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="568ee-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="568ee-106">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="568ee-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="568ee-107">Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.</span><span class="sxs-lookup"><span data-stu-id="568ee-107">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="568ee-108">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="568ee-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="568ee-109">[Tendências](insights-trending.md) – retorna a documentos do OneDrive e de sites do SharePoint de tendências de um usuário à sua volta.</span><span class="sxs-lookup"><span data-stu-id="568ee-109">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="568ee-110">[Usado](insights-used.md) - Retornar documentos visualizados e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="568ee-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="568ee-111">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="568ee-111">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="568ee-112">[Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="568ee-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="568ee-113">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="568ee-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="568ee-114">Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="568ee-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="568ee-115">O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="568ee-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="568ee-116">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="568ee-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="568ee-117">Relações</span><span class="sxs-lookup"><span data-stu-id="568ee-117">Relationships</span></span>

| <span data-ttu-id="568ee-118">Relação</span><span class="sxs-lookup"><span data-stu-id="568ee-118">Relationship</span></span>      | <span data-ttu-id="568ee-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="568ee-119">Type</span></span>          | <span data-ttu-id="568ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="568ee-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="568ee-121">tendências</span><span class="sxs-lookup"><span data-stu-id="568ee-121">trending</span></span>      | <span data-ttu-id="568ee-122">[tendências](insights-trending.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="568ee-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="568ee-123">Relação calculada identificando documentos mais populares.</span><span class="sxs-lookup"><span data-stu-id="568ee-123">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="568ee-124">Os documentos mais populares podem ser armazenados no OneDrive ou em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="568ee-124">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="568ee-125">usado</span><span class="sxs-lookup"><span data-stu-id="568ee-125">used</span></span>      | <span data-ttu-id="568ee-126">[usedInsight](insights-used.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="568ee-126">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="568ee-127">Relação calculada para identificar documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="568ee-127">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="568ee-128">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="568ee-128">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="568ee-129">compartilhado</span><span class="sxs-lookup"><span data-stu-id="568ee-129">shared</span></span>        | <span data-ttu-id="568ee-130">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="568ee-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="568ee-131">Relação calculada identificando documentos mais populares compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="568ee-131">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="568ee-132">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="568ee-132">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="568ee-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="568ee-133">JSON representation</span></span>

<span data-ttu-id="568ee-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="568ee-134">Here is a JSON representation of the resource</span></span>
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
