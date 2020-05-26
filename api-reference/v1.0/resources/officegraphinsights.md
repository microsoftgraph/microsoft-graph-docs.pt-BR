---
title: tipo de recurso officeGraphInsights
description: Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina. Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bfc058612b883ae51a1a674663c2704c4f4cde88
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226893"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="efa9d-104">tipo de recurso officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="efa9d-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="efa9d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa9d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efa9d-106">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="efa9d-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="efa9d-107">Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.</span><span class="sxs-lookup"><span data-stu-id="efa9d-107">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="efa9d-108">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="efa9d-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="efa9d-109">[Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="efa9d-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="efa9d-110">[Usado](insights-used.md) - retorna documentos visualizados ou modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="efa9d-110">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="efa9d-111">Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="efa9d-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="efa9d-112">[Compartilhado](insights-shared.md) - retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="efa9d-112">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="efa9d-113">Os documentos podem ser compartilhados como URLs, anexos de arquivo, anexos de referência aos arquivos do OneDrive for Business e SharePoint encontrados nas mensagens e reuniões do Outlook.</span><span class="sxs-lookup"><span data-stu-id="efa9d-113">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="efa9d-114">Cada opinião é retornada com um **resourceVisualization** e Tipo de valor complexo (CVT) **resourceReference**.</span><span class="sxs-lookup"><span data-stu-id="efa9d-114">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="efa9d-115">O CVT **resourceVisualization** contém propriedades como **título** e **previewImageUrl**.</span><span class="sxs-lookup"><span data-stu-id="efa9d-115">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="efa9d-116">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="efa9d-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="efa9d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="efa9d-117">Relationships</span></span>

| <span data-ttu-id="efa9d-118">Relação</span><span class="sxs-lookup"><span data-stu-id="efa9d-118">Relationship</span></span>      | <span data-ttu-id="efa9d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa9d-119">Type</span></span>          | <span data-ttu-id="efa9d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa9d-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="efa9d-121">tendências</span><span class="sxs-lookup"><span data-stu-id="efa9d-121">trending</span></span>      | <span data-ttu-id="efa9d-122">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="efa9d-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="efa9d-123">Relacionamento calculado que identifica documentos de tendências em torno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efa9d-123">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="efa9d-124">Os documentos de tendência são calculados com base na atividade da rede de pessoas mais próximas do usuário e incluem arquivos armazenados no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="efa9d-124">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="efa9d-125">As informações de tendências ajudam o usuário a descobrir o conteúdo potencialmente útil que ele tem acesso, mas nunca viu antes.</span><span class="sxs-lookup"><span data-stu-id="efa9d-125">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="efa9d-126">usado</span><span class="sxs-lookup"><span data-stu-id="efa9d-126">used</span></span>      | <span data-ttu-id="efa9d-127">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="efa9d-127">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="efa9d-128">Relacionamento calculado que identifica os documentos mais recentes exibidos ou modificados por um usuário, incluindo documentos do OneDrive for Business e do SharePoint, classificados por tempo de uso recente.</span><span class="sxs-lookup"><span data-stu-id="efa9d-128">Calculated relationship identifying the latest documents viewed or modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="efa9d-129">compartilhado</span><span class="sxs-lookup"><span data-stu-id="efa9d-129">shared</span></span>        | <span data-ttu-id="efa9d-130">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="efa9d-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="efa9d-131">Relacionamento calculado identificando documentos compartilhados com ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="efa9d-131">Calculated relationship identifying documents shared with or by the user.</span></span> <span data-ttu-id="efa9d-132">Isso inclui URLs, anexos de arquivo e anexos de referência aos arquivos do OneDrive for Business e SharePoint encontrados nas mensagens e reuniões do Outlook.</span><span class="sxs-lookup"><span data-stu-id="efa9d-132">This includes URLs, file attachments, and reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span> <span data-ttu-id="efa9d-133">Isso também inclui URLs e anexos de referência para conversas do Teams.</span><span class="sxs-lookup"><span data-stu-id="efa9d-133">This also includes URLs and reference attachments to Teams conversations.</span></span> <span data-ttu-id="efa9d-134">Ordenado por tempo de compartilhamento recente.</span><span class="sxs-lookup"><span data-stu-id="efa9d-134">Ordered by recency of share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efa9d-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efa9d-135">JSON representation</span></span>

<span data-ttu-id="efa9d-136">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="efa9d-136">Here is a JSON representation of the resource</span></span>
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
