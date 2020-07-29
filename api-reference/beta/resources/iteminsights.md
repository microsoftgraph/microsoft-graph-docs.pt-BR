---
title: tipo de recurso itemInsights
description: Relacionamentos entre um usuário e itens como documentos do OneDrive for Business, calculados usando análises avançadas e técnicas de aprendizado de máquina. Por exemplo, você pode identificar tendências de documentos do OneDrive for Business entre usuários à sua volta.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e5f0e525f95f988e7cb90c454285d2ecdb6b1072
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434995"
---
# <a name="iteminsights-resource-type"></a><span data-ttu-id="27cb2-104">tipo de recurso itemInsights</span><span class="sxs-lookup"><span data-stu-id="27cb2-104">itemInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27cb2-105">Relacionamentos entre um usuário e itens como documentos do OneDrive for Business, calculados usando análises avançadas e técnicas de aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="27cb2-105">Relationships between a user and items such as OneDrive for Business documents, calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="27cb2-106">Por exemplo, você pode identificar tendências de documentos do OneDrive for Business entre usuários à sua volta.</span><span class="sxs-lookup"><span data-stu-id="27cb2-106">You can, for example, identify OneDrive for Business documents trending around users.</span></span> <span data-ttu-id="27cb2-107">Derivados do [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="27cb2-107">Derived from [officeGraphInsights](officegraphinsights.md).</span></span>

<span data-ttu-id="27cb2-108">Informações são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="27cb2-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="27cb2-109">[Tendências](insights-trending.md) - retorna documentos do OneDrive for Business e de sites do SharePoint tendendo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="27cb2-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="27cb2-110">[Usadas](insights-used.md) - retorna documentos exibidos e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="27cb2-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="27cb2-111">Inclui documentos que o usuário usou no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27cb2-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="27cb2-112">[Compartilhado](insights-shared.md) -retornará documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="27cb2-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="27cb2-113">Documentos podem ser compartilhados como anexos de email ou links do OneDrive para Business enviados por email.</span><span class="sxs-lookup"><span data-stu-id="27cb2-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="27cb2-114">Cada ideia é retornada com um tipo de valor complexo (CVT) `resourceVisualization` e `resourceReference`.</span><span class="sxs-lookup"><span data-stu-id="27cb2-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="27cb2-115">O resourceVisualization CVT contém propriedades, como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="27cb2-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="27cb2-116">A Microsoft usa as propriedades de visualização para renderizar os arquivos em experiências como o Office Delve.</span><span class="sxs-lookup"><span data-stu-id="27cb2-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

### <a name="limiting-item-insights"></a><span data-ttu-id="27cb2-117">Limitando as informações do item</span><span class="sxs-lookup"><span data-stu-id="27cb2-117">Limiting item insights</span></span>

<span data-ttu-id="27cb2-118">Atualize [itemInsightsSettings](iteminsightssettings.md) para desabilitar as informações do item em um grupo específico do Azure AD ou em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="27cb2-118">Update [itemInsightsSettings](iteminsightssettings.md) to disable item insights for a specific Azure AD group or an entire organization.</span></span> <span data-ttu-id="27cb2-119">Para obter mais detalhes, confira [personalizar política de informações](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="27cb2-119">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span>

## <a name="relationships"></a><span data-ttu-id="27cb2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="27cb2-120">Relationships</span></span>

| <span data-ttu-id="27cb2-121">Relação</span><span class="sxs-lookup"><span data-stu-id="27cb2-121">Relationship</span></span>      | <span data-ttu-id="27cb2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="27cb2-122">Type</span></span>          | <span data-ttu-id="27cb2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="27cb2-123">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="27cb2-124">tendências</span><span class="sxs-lookup"><span data-stu-id="27cb2-124">trending</span></span>      | <span data-ttu-id="27cb2-125">coleção [tendências](insights-trending.md) </span><span class="sxs-lookup"><span data-stu-id="27cb2-125">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="27cb2-126">Relacionamento calculado que identifica documentos de tendências em torno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="27cb2-126">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="27cb2-127">Os documentos de tendência são calculados com base na atividade da rede de pessoas mais próximas do usuário e incluem arquivos armazenados no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27cb2-127">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="27cb2-128">As informações de tendências ajudam o usuário a descobrir o conteúdo potencialmente útil que ele tem acesso, mas nunca viu antes.</span><span class="sxs-lookup"><span data-stu-id="27cb2-128">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="27cb2-129">usado</span><span class="sxs-lookup"><span data-stu-id="27cb2-129">used</span></span>      | <span data-ttu-id="27cb2-130">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="27cb2-130">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="27cb2-131">Relacionamento calculado que identifica os documentos mais recentes exibidos e modificados por um usuário, incluindo documentos do OneDrive for Business e do SharePoint, classificados por tempo de uso recente.</span><span class="sxs-lookup"><span data-stu-id="27cb2-131">Calculated relationship identifying the latest documents viewed and modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="27cb2-132">compartilhado</span><span class="sxs-lookup"><span data-stu-id="27cb2-132">shared</span></span>        | <span data-ttu-id="27cb2-133">coleção [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="27cb2-133">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="27cb2-134">O relacionamento calculado para identificar documentos compartilhados com ou pelo usuário inclui anexos de arquivo em emails e reuniões, além de URLs e anexos de referência aos arquivos do OneDrive for Business e do SharePoint encontrados em emails, reuniões e conversas do Teams.</span><span class="sxs-lookup"><span data-stu-id="27cb2-134">Calculated relationship identifying documents shared with or by the user, includes file attachments in emails and meetings, as well as URLs and Reference attachments to OneDrive for Business and SharePoint files found in emails, meetings, and Teams conversations.</span></span> <span data-ttu-id="27cb2-135">Ordenado por tempo de compartilhamento recente.</span><span class="sxs-lookup"><span data-stu-id="27cb2-135">Ordered by recency of share.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="27cb2-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27cb2-136">JSON representation</span></span>

<span data-ttu-id="27cb2-137">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="27cb2-137">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
