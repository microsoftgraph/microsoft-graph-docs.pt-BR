---
title: tipo de recurso officeGraphInsights
description: Representa o tipo base para itemInsights. officeGraphInsights é para fins de compatibilidade com versões anteriores da API do insights. Use apenas itemInsights ao acessar a API do insights.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f10d12a0014b38fbe954f957987e585dafa63a2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092325"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="07355-105">tipo de recurso officeGraphInsights</span><span class="sxs-lookup"><span data-stu-id="07355-105">officeGraphInsights resource type</span></span>

<span data-ttu-id="07355-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07355-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07355-107">Use [itemInsights](iteminsights.md) no lugar de **officeGraphInsights** para acessar a API do insights.</span><span class="sxs-lookup"><span data-stu-id="07355-107">Use [itemInsights](iteminsights.md) in place of **officeGraphInsights** to access the insights API.</span></span>

<span data-ttu-id="07355-108">**officeGraphInsights** é para fins de compatibilidade com versões anteriores da API do insights.</span><span class="sxs-lookup"><span data-stu-id="07355-108">**officeGraphInsights** is for backward compatibility from earlier versions of the insights API.</span></span> <span data-ttu-id="07355-109">É o tipo de base para [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="07355-109">It is the base type for [itemInsights](iteminsights.md).</span></span>

<span data-ttu-id="07355-110">Ideias são relações calculadas usando análises e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="07355-110">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="07355-111">Por exemplo, você pode identificar documentos do OneDrive for Business que se aproximam dos usuários.</span><span class="sxs-lookup"><span data-stu-id="07355-111">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="07355-112">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="07355-112">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="07355-113">[Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="07355-113">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="07355-114">[Usado](insights-used.md) - retorna documentos visualizados ou modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="07355-114">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="07355-115">Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07355-115">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="07355-116">[Compartilhado](insights-shared.md) - retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="07355-116">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="07355-117">Os documentos podem ser compartilhados como URLs, anexos de arquivo, anexos de referência aos arquivos do OneDrive for Business e SharePoint encontrados nas mensagens e reuniões do Outlook.</span><span class="sxs-lookup"><span data-stu-id="07355-117">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="07355-118">Cada opinião é retornada com um **resourceVisualization** e Tipo de valor complexo (CVT) **resourceReference**.</span><span class="sxs-lookup"><span data-stu-id="07355-118">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="07355-119">O CVT **resourceVisualization** contém propriedades como **título** e **previewImageUrl**.</span><span class="sxs-lookup"><span data-stu-id="07355-119">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="07355-120">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="07355-120">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="07355-121">Relações</span><span class="sxs-lookup"><span data-stu-id="07355-121">Relationships</span></span>

| <span data-ttu-id="07355-122">Relação</span><span class="sxs-lookup"><span data-stu-id="07355-122">Relationship</span></span>      | <span data-ttu-id="07355-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="07355-123">Type</span></span>          | <span data-ttu-id="07355-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="07355-124">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="07355-125">tendências</span><span class="sxs-lookup"><span data-stu-id="07355-125">trending</span></span>      | <span data-ttu-id="07355-126">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="07355-126">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="07355-127">Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="07355-127">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="07355-128">usado</span><span class="sxs-lookup"><span data-stu-id="07355-128">used</span></span>      | <span data-ttu-id="07355-129">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="07355-129">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="07355-130">Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="07355-130">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="07355-131">compartilhado</span><span class="sxs-lookup"><span data-stu-id="07355-131">shared</span></span>        | <span data-ttu-id="07355-132">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="07355-132">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="07355-133">Acessar essa propriedade a partir do tipo derivado [itemInsights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="07355-133">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="07355-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07355-134">JSON representation</span></span>

<span data-ttu-id="07355-135">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="07355-135">Here is a JSON representation of the resource</span></span>
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



