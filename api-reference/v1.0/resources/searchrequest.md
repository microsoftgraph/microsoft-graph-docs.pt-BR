---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f673c551ce27c16fd4fddabc26e55cd234a9f19e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377956"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="37455-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="37455-104">searchRequest resource type</span></span>

<span data-ttu-id="37455-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37455-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37455-106">Uma solicitação de pesquisa formatada em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="37455-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="37455-107">O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, as opções de classificação, as agregações e os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="37455-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="37455-108">Confira [exemplos](#see-also) de solicitações de pesquisa em vários recursos.</span><span class="sxs-lookup"><span data-stu-id="37455-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="37455-109">Esteja ciente das [limitações conhecidas](search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="37455-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="37455-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37455-110">Properties</span></span>

| <span data-ttu-id="37455-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37455-111">Property</span></span>     | <span data-ttu-id="37455-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="37455-112">Type</span></span>        | <span data-ttu-id="37455-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="37455-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="37455-114">contentSources</span><span class="sxs-lookup"><span data-stu-id="37455-114">contentSources</span></span>|<span data-ttu-id="37455-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37455-115">String collection</span></span>|<span data-ttu-id="37455-116">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="37455-116">Contains the connection to be targeted.</span></span>|
|<span data-ttu-id="37455-117">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="37455-117">enableTopResults</span></span>|<span data-ttu-id="37455-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="37455-118">Boolean</span></span>|<span data-ttu-id="37455-119">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="37455-119">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="37455-120">Esta propriedade só é aplicável a entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="37455-120">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="37455-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37455-121">Optional.</span></span>|
|<span data-ttu-id="37455-122">entityTypes</span><span class="sxs-lookup"><span data-stu-id="37455-122">entityTypes</span></span>|<span data-ttu-id="37455-123">coleção entityType</span><span class="sxs-lookup"><span data-stu-id="37455-123">entityType collection</span></span>| <span data-ttu-id="37455-124">Um ou mais tipos de recursos esperados na resposta.</span><span class="sxs-lookup"><span data-stu-id="37455-124">One or more types of resources expected in the response.</span></span> <span data-ttu-id="37455-125">Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`.</span><span class="sxs-lookup"><span data-stu-id="37455-125">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`.</span></span> <span data-ttu-id="37455-126">Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para as combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="37455-126">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="37455-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37455-127">Required.</span></span>|
|<span data-ttu-id="37455-128">campos</span><span class="sxs-lookup"><span data-stu-id="37455-128">fields</span></span>|<span data-ttu-id="37455-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37455-129">String collection</span></span> |<span data-ttu-id="37455-130">Contém os campos a serem retornados para cada objeto de recurso especificado em **EntityTypes**, permitindo a personalização dos campos retornados por padrão, caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e do onedrive.</span><span class="sxs-lookup"><span data-stu-id="37455-130">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive.</span></span> <span data-ttu-id="37455-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37455-131">Optional.</span></span>|
|<span data-ttu-id="37455-132">from</span><span class="sxs-lookup"><span data-stu-id="37455-132">from</span></span>|<span data-ttu-id="37455-133">Int32</span><span class="sxs-lookup"><span data-stu-id="37455-133">Int32</span></span>|<span data-ttu-id="37455-134">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="37455-134">Specifies the offset for the search results.</span></span> <span data-ttu-id="37455-135">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="37455-135">Offset 0 returns the very first result.</span></span> <span data-ttu-id="37455-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37455-136">Optional.</span></span>|
|<span data-ttu-id="37455-137">consulta</span><span class="sxs-lookup"><span data-stu-id="37455-137">query</span></span>|[<span data-ttu-id="37455-138">searchQuery</span><span class="sxs-lookup"><span data-stu-id="37455-138">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="37455-139">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="37455-139">Contains the query terms.</span></span> <span data-ttu-id="37455-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37455-140">Required.</span></span>|
|<span data-ttu-id="37455-141">size</span><span class="sxs-lookup"><span data-stu-id="37455-141">size</span></span>|<span data-ttu-id="37455-142">Int32</span><span class="sxs-lookup"><span data-stu-id="37455-142">Int32</span></span>|<span data-ttu-id="37455-143">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="37455-143">The size of the page to be retrieved.</span></span> <span data-ttu-id="37455-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="37455-144">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37455-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37455-145">JSON representation</span></span>

<span data-ttu-id="37455-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37455-146">The following is a JSON representation of the resource.</span></span>

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="37455-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="37455-147">See also</span></span>
- <span data-ttu-id="37455-148">[Mensagens de email](/graph/search-concept-messages) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="37455-148">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="37455-149">[Eventos de calendário](/graph/search-concept-events) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="37455-149">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="37455-150">Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="37455-150">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


