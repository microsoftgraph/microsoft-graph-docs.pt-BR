---
title: tipo de recurso de ideias
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551894"
---
# <a name="insights-resource-type"></a><span data-ttu-id="d5943-104">tipo de recurso de ideias</span><span class="sxs-lookup"><span data-stu-id="d5943-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5943-105">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="d5943-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="d5943-106">Por exemplo, você pode identificar tendências de documentos do OneDrive com usuários à sua volta.</span><span class="sxs-lookup"><span data-stu-id="d5943-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="d5943-107">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="d5943-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="d5943-108">[Tendências](insights-trending.md) – retorna a documentos do OneDrive e de sites do SharePoint de tendências de um usuário à sua volta.</span><span class="sxs-lookup"><span data-stu-id="d5943-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="d5943-109">[Usado](insights-used.md) - Retornar documentos visualizados e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5943-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="d5943-110">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="d5943-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="d5943-111">[Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5943-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="d5943-112">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="d5943-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="d5943-113">Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="d5943-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="d5943-114">O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="d5943-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="d5943-115">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="d5943-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="d5943-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d5943-116">Relationships</span></span>

| <span data-ttu-id="d5943-117">Relação</span><span class="sxs-lookup"><span data-stu-id="d5943-117">Relationship</span></span>      | <span data-ttu-id="d5943-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5943-118">Type</span></span>          | <span data-ttu-id="d5943-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5943-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="d5943-120">trending</span><span class="sxs-lookup"><span data-stu-id="d5943-120">trending</span></span>      | <span data-ttu-id="d5943-121">Coleção [Tendências](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="d5943-121">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="d5943-122">Relação calculada identificando documentos mais populares.</span><span class="sxs-lookup"><span data-stu-id="d5943-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="d5943-123">Os documentos mais populares podem ser armazenados no OneDrive ou em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d5943-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="d5943-124">used</span><span class="sxs-lookup"><span data-stu-id="d5943-124">used</span></span>      | <span data-ttu-id="d5943-125">Coleção [Usado](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="d5943-125">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="d5943-126">Relação calculada para identificar documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5943-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="d5943-127">Inclui documentos que o usuário usou no OneDrive for Business, SharePoint, aberto como anexos de email e anexos de link de fontes como o Box, DropBox e Google Drive.</span><span class="sxs-lookup"><span data-stu-id="d5943-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="d5943-128">shared</span><span class="sxs-lookup"><span data-stu-id="d5943-128">shared</span></span>        | <span data-ttu-id="d5943-129">Coleção [compartilhado](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="d5943-129">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="d5943-130">Relação calculada identificando documentos mais populares compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5943-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="d5943-131">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="d5943-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="d5943-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5943-132">JSON representation</span></span>

<span data-ttu-id="d5943-133">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d5943-133">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
