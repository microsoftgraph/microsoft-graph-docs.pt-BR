---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 04bdca98f4676454a72e503e8bfe747bbda306cc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372689"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="c1590-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="c1590-104">searchRequest resource type</span></span>

<span data-ttu-id="c1590-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1590-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="c1590-106">Uma solicitação de pesquisa formatada em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="c1590-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="c1590-107">O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, as opções de classificação, as agregações e os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="c1590-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="c1590-108">Confira [exemplos](#see-also) de solicitações de pesquisa em vários recursos.</span><span class="sxs-lookup"><span data-stu-id="c1590-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="c1590-109">Esteja ciente das [limitações conhecidas](search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c1590-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="c1590-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1590-110">Properties</span></span>

| <span data-ttu-id="c1590-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1590-111">Property</span></span>     | <span data-ttu-id="c1590-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1590-112">Type</span></span>        | <span data-ttu-id="c1590-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1590-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="c1590-114">aggregations</span><span class="sxs-lookup"><span data-stu-id="c1590-114">aggregations</span></span>|<span data-ttu-id="c1590-115">coleção [aggregationOption](aggregationOption.md)</span><span class="sxs-lookup"><span data-stu-id="c1590-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="c1590-116">Especifica agregações (também conhecidas como refinadores) a serem retornadas junto com os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c1590-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="c1590-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-117">Optional.</span></span>|
|<span data-ttu-id="c1590-118">aggregationFilters</span><span class="sxs-lookup"><span data-stu-id="c1590-118">aggregationFilters</span></span>|<span data-ttu-id="c1590-119">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1590-119">String collection</span></span>|<span data-ttu-id="c1590-120">Contém um ou mais filtros para obter os resultados da pesquisa agregados e filtrados para um valor específico de um campo.</span><span class="sxs-lookup"><span data-stu-id="c1590-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="c1590-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-121">Optional.</span></span><br><span data-ttu-id="c1590-122">Crie este filtro com base em uma pesquisa anterior que seja agregada pelo mesmo campo.</span><span class="sxs-lookup"><span data-stu-id="c1590-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="c1590-123">Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres na propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="c1590-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="c1590-124">Por exemplo, a pesquisa e agregação de itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de arquivo `docx` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c1590-124">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="c1590-125">Você pode usar convenientemente o **aggregationFilterToken** retornado para este **searchBucket** em uma consulta de pesquisa e filtro de correspondência subsequentes correspondem a itens de unidade do `docx` tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c1590-125">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="c1590-126">O [exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) e o [exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.</span><span class="sxs-lookup"><span data-stu-id="c1590-126">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="c1590-127">contentSources</span><span class="sxs-lookup"><span data-stu-id="c1590-127">contentSources</span></span>|<span data-ttu-id="c1590-128">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1590-128">String collection</span></span>|<span data-ttu-id="c1590-129">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="c1590-129">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="c1590-130">Respeita o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores.</span><span class="sxs-lookup"><span data-stu-id="c1590-130">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="c1590-131">Observação: contentSource só é aplicável quando entityType = `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="c1590-131">Note : contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="c1590-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-132">Optional.</span></span>|
|<span data-ttu-id="c1590-133">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="c1590-133">enableTopResults</span></span>|<span data-ttu-id="c1590-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1590-134">Boolean</span></span>|<span data-ttu-id="c1590-135">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="c1590-135">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="c1590-136">Esta propriedade só é aplicável a entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="c1590-136">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="c1590-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-137">Optional.</span></span>|
|<span data-ttu-id="c1590-138">entityTypes</span><span class="sxs-lookup"><span data-stu-id="c1590-138">entityTypes</span></span>|<span data-ttu-id="c1590-139">coleção entityType</span><span class="sxs-lookup"><span data-stu-id="c1590-139">entityType collection</span></span>| <span data-ttu-id="c1590-140">Um ou mais tipos de recursos esperados na resposta.</span><span class="sxs-lookup"><span data-stu-id="c1590-140">One or more types of resources expected in the response.</span></span> <span data-ttu-id="c1590-141">Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="c1590-141">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="c1590-142">Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para as combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c1590-142">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="c1590-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1590-143">Required.</span></span>|
|<span data-ttu-id="c1590-144">campos</span><span class="sxs-lookup"><span data-stu-id="c1590-144">fields</span></span>|<span data-ttu-id="c1590-145">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1590-145">String collection</span></span> |<span data-ttu-id="c1590-146">Contém os campos a serem retornados para cada objeto de recurso especificado em **EntityTypes**, permitindo a personalização dos campos retornados por padrão, caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e do onedrive, ou campos personalizados no **externalItem** a partir de conteúdo ingerido por conectores do Graph.</span><span class="sxs-lookup"><span data-stu-id="c1590-146">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content ingested by Graph connectors.</span></span> <span data-ttu-id="c1590-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-147">Optional.</span></span>|
|<span data-ttu-id="c1590-148">from</span><span class="sxs-lookup"><span data-stu-id="c1590-148">from</span></span>|<span data-ttu-id="c1590-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c1590-149">Int32</span></span>|<span data-ttu-id="c1590-150">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c1590-150">Specifies the offset for the search results.</span></span> <span data-ttu-id="c1590-151">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="c1590-151">Offset 0 returns the very first result.</span></span> <span data-ttu-id="c1590-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-152">Optional.</span></span>|
|<span data-ttu-id="c1590-153">consulta</span><span class="sxs-lookup"><span data-stu-id="c1590-153">query</span></span>|[<span data-ttu-id="c1590-154">searchQuery</span><span class="sxs-lookup"><span data-stu-id="c1590-154">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="c1590-155">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="c1590-155">Contains the query terms.</span></span> <span data-ttu-id="c1590-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1590-156">Required.</span></span>|
|<span data-ttu-id="c1590-157">size</span><span class="sxs-lookup"><span data-stu-id="c1590-157">size</span></span>|<span data-ttu-id="c1590-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c1590-158">Int32</span></span>|<span data-ttu-id="c1590-159">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="c1590-159">The size of the page to be retrieved.</span></span> <span data-ttu-id="c1590-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-160">Optional.</span></span>|
|<span data-ttu-id="c1590-161">sortproperties</span><span class="sxs-lookup"><span data-stu-id="c1590-161">sortProperties</span></span>|<span data-ttu-id="c1590-162">coleção [SortProperty](sortProperty.md)</span><span class="sxs-lookup"><span data-stu-id="c1590-162">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="c1590-163">Contém a coleção ordenada de campos e direção para classificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="c1590-163">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="c1590-164">Pode haver no máximo 5 Propriedades de classificação na coleção.</span><span class="sxs-lookup"><span data-stu-id="c1590-164">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="c1590-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1590-165">Optional.</span></span>|
|<span data-ttu-id="c1590-166">stored_fields (preterido)</span><span class="sxs-lookup"><span data-stu-id="c1590-166">stored_fields (deprecated)</span></span>|<span data-ttu-id="c1590-167">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1590-167">String collection</span></span> |<span data-ttu-id="c1590-168">Agora, ela é substituída pela propriedade **Fields** .</span><span class="sxs-lookup"><span data-stu-id="c1590-168">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c1590-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1590-169">JSON representation</span></span>

<span data-ttu-id="c1590-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1590-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "aggregationFilters": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a><span data-ttu-id="c1590-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1590-171">See also</span></span>
- <span data-ttu-id="c1590-172">[Mensagens de email](/graph/search-concept-messages) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c1590-172">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="c1590-173">[Eventos de calendário](/graph/search-concept-events) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c1590-173">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="c1590-174">Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="c1590-174">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="c1590-175">Dados [de tipos personalizados de pesquisa (conectores do gráfico)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="c1590-175">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="c1590-176">[Classificar](/graph/search-concept-sort) resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c1590-176">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="c1590-177">Usar [agregações](/graph/search-concept-aggregations) para refinar os resultados da pesquisa</span><span class="sxs-lookup"><span data-stu-id="c1590-177">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


