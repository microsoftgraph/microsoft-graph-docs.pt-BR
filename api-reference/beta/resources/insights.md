---
title: tipo de recurso de ideias de pesquisas
description: Ideias são relações calculadas usando análises avançadas e técnicas de aprendizagem da máquina. Você pode, por exemplo, identificar documentos OneDrive tendências em torno de usuários.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938311"
---
# <a name="insights-resource-type"></a><span data-ttu-id="75c89-104">tipo de recurso de ideias de pesquisas</span><span class="sxs-lookup"><span data-stu-id="75c89-104">insights resource type</span></span>

> <span data-ttu-id="75c89-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75c89-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75c89-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75c89-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75c89-107">Ideias são relações calculadas usando análises avançadas e técnicas de aprendizagem da máquina.</span><span class="sxs-lookup"><span data-stu-id="75c89-107">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="75c89-108">Você pode, por exemplo, identificar documentos OneDrive tendências em torno de usuários.</span><span class="sxs-lookup"><span data-stu-id="75c89-108">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="75c89-109">Ideias são retornadas pelas seguintes APIs:</span><span class="sxs-lookup"><span data-stu-id="75c89-109">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="75c89-110">[Tendência](insights-trending.md) - retornará documentos do OneDrive e de sites do SharePoint tendências em torno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="75c89-110">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="75c89-111">[Usado](insights-used.md) - retornará documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="75c89-111">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="75c89-112">Inclui os documentos que o usuário tiver usado no OneDrive for Business, SharePoint, abertos como anexos de email e como anexos de link de fontes como caixa, pasta de recados e Google unidade.</span><span class="sxs-lookup"><span data-stu-id="75c89-112">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="75c89-113">[Shared](insights-shared.md) - retorna documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="75c89-113">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="75c89-114">Documentos podem ser compartilhados como anexos de email ou OneDrive for Business vincula emails enviados no.</span><span class="sxs-lookup"><span data-stu-id="75c89-114">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="75c89-115">Cada insight é retornado com um `resourceVisualization` e `resourceReference` o tipo de valor complexa (CVT).</span><span class="sxs-lookup"><span data-stu-id="75c89-115">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="75c89-116">O resourceVisualization CVT contém propriedades tais como `title` e `previewImageUrl`.</span><span class="sxs-lookup"><span data-stu-id="75c89-116">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="75c89-117">A Microsoft usa as propriedades de visualização para processar os arquivos em experiências como Office me aprofundar.</span><span class="sxs-lookup"><span data-stu-id="75c89-117">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="75c89-118">Relações</span><span class="sxs-lookup"><span data-stu-id="75c89-118">Relationships</span></span>

| <span data-ttu-id="75c89-119">Relação</span><span class="sxs-lookup"><span data-stu-id="75c89-119">Relationship</span></span>      | <span data-ttu-id="75c89-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="75c89-120">Type</span></span>          | <span data-ttu-id="75c89-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="75c89-121">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="75c89-122">análise de tendências</span><span class="sxs-lookup"><span data-stu-id="75c89-122">trending</span></span>      | <span data-ttu-id="75c89-123">Coleção de [tendência](insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="75c89-123">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="75c89-124">Relacionamento calculado identificar tendências de documentos.</span><span class="sxs-lookup"><span data-stu-id="75c89-124">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="75c89-125">Tendências de documentos podem ser armazenados em OneDrive ou em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="75c89-125">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="75c89-126">used</span><span class="sxs-lookup"><span data-stu-id="75c89-126">used</span></span>      | <span data-ttu-id="75c89-127">Coleção [usado](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="75c89-127">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="75c89-128">Calculado relação identificar documentos exibidos e modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="75c89-128">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="75c89-129">Inclui os documentos que o usuário tiver usado no OneDrive for Business, SharePoint, abertos como anexos de email e como anexos de link de fontes como caixa, pasta de recados e Google unidade.</span><span class="sxs-lookup"><span data-stu-id="75c89-129">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="75c89-130">shared</span><span class="sxs-lookup"><span data-stu-id="75c89-130">shared</span></span>        | <span data-ttu-id="75c89-131">Coleção [compartilhados](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="75c89-131">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="75c89-132">Relacionamento calculado identificando documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="75c89-132">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="75c89-133">Documentos podem ser compartilhados como anexos de email ou OneDrive for Business vincula emails enviados no.</span><span class="sxs-lookup"><span data-stu-id="75c89-133">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="75c89-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75c89-134">JSON representation</span></span>

<span data-ttu-id="75c89-135">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="75c89-135">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
