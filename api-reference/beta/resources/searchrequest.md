---
title: Tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta. Ele contém o tipo de entidade esperado na resposta, as fontes subjacentes, os parâmetros de paging, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3bda8b317e1bc42e21943c23ca8a841572cf8cd0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883183"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="7cdf8-104">Tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="7cdf8-104">searchRequest resource type</span></span>

<span data-ttu-id="7cdf8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cdf8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="7cdf8-106">Uma solicitação de pesquisa formatada em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-106">A search request formatted in a JSON blob.</span></span> 

<span data-ttu-id="7cdf8-107">O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paging, as opções de classificação, as agregação e os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-107">The JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, sort options, requested aggregations and fields, and actual search query.</span></span> <span data-ttu-id="7cdf8-108">Veja [exemplos de](#see-also) solicitações de pesquisa em vários recursos.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-108">See [examples](#see-also) of search requests on various resources.</span></span>

> [!NOTE]
> <span data-ttu-id="7cdf8-109">Esteja ciente das [limitações conhecidas em](search-api-overview.md#known-limitations) pesquisar combinações específicas de tipos de entidade e classificar ou agregar resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-109">Be aware of [known limitations](search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span>


## <a name="properties"></a><span data-ttu-id="7cdf8-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cdf8-110">Properties</span></span>

| <span data-ttu-id="7cdf8-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cdf8-111">Property</span></span>     | <span data-ttu-id="7cdf8-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cdf8-112">Type</span></span>        | <span data-ttu-id="7cdf8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cdf8-113">Description</span></span> |
|:-------------|:------------|:------------|:------------|
|<span data-ttu-id="7cdf8-114">aggregations</span><span class="sxs-lookup"><span data-stu-id="7cdf8-114">aggregations</span></span>|<span data-ttu-id="7cdf8-115">[Coleção aggregationOption](aggregationOption.md)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-115">[aggregationOption](aggregationOption.md) collection</span></span>|<span data-ttu-id="7cdf8-116">Especifica as agregação (também conhecidas como refinadores) a serem retornadas junto com os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-116">Specifies aggregations (also known as refiners) to be returned alongside search results.</span></span> <span data-ttu-id="7cdf8-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-117">Optional.</span></span>|
|<span data-ttu-id="7cdf8-118">aggregationFilters</span><span class="sxs-lookup"><span data-stu-id="7cdf8-118">aggregationFilters</span></span>|<span data-ttu-id="7cdf8-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cdf8-119">String collection</span></span>|<span data-ttu-id="7cdf8-120">Contém um ou mais filtros para obter resultados de pesquisa agregados e filtrados para um valor específico de um campo.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-120">Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field.</span></span> <span data-ttu-id="7cdf8-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-121">Optional.</span></span><br><span data-ttu-id="7cdf8-122">Crie esse filtro com base em uma pesquisa anterior que seja agregada pelo mesmo campo.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-122">Build this filter based on a prior search that aggregates by the same field.</span></span> <span data-ttu-id="7cdf8-123">Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **\\ "{field}: "{aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-123">From the response of the prior search, identify the [searchBucket](searchBucket.md) that filters results to the specific value of the field, use the string in its **aggregationFilterToken** property, and build an aggregation filter string in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <br><span data-ttu-id="7cdf8-124">Se vários valores para o mesmo campo precisam ser fornecidos, use as cadeias de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **\\ "{field}:or( "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-124">If multiple values for the same field need to be provided, use the strings in its **aggregationFilterToken** property and build an aggregation filter string in the format **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span> <br><span data-ttu-id="7cdf8-125">Por exemplo, pesquisar e agregar itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de `docx` arquivo na resposta.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-125">For example, searching and aggregating drive items by file type returns a **searchBucket** for the file type `docx` in the response.</span></span> <span data-ttu-id="7cdf8-126">Você pode usar convenientemente o **aggregationFilterToken** retornado para esse **searchBucket** em uma consulta de pesquisa subsequente e o filtro corresponde aos itens de unidade do tipo `docx` de arquivo.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-126">You can conveniently use the **aggregationFilterToken** returned for this **searchBucket** in a subsequent search query and filter matches down to drive items of the `docx` file type.</span></span> <span data-ttu-id="7cdf8-127">[O Exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) e [o exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-127">[Example 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) and [example 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) show the actual requests and responses.</span></span>|
|<span data-ttu-id="7cdf8-128">contentSources</span><span class="sxs-lookup"><span data-stu-id="7cdf8-128">contentSources</span></span>|<span data-ttu-id="7cdf8-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cdf8-129">String collection</span></span>|<span data-ttu-id="7cdf8-130">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-130">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="7cdf8-131">Respeita o seguinte formato: `/external/connections/connectionid` onde `connectionid` ConnectionId é definido na Administração de Conectores.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-131">Respects the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId defined in the Connectors Administration.</span></span> <br> <span data-ttu-id="7cdf8-132">Observação: contentSource só é aplicável quando entityType= `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="7cdf8-132">Note : contentSource is only applicable when entityType=`externalItem`.</span></span> <span data-ttu-id="7cdf8-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-133">Optional.</span></span>|
|<span data-ttu-id="7cdf8-134">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="7cdf8-134">enableTopResults</span></span>|<span data-ttu-id="7cdf8-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="7cdf8-135">Boolean</span></span>|<span data-ttu-id="7cdf8-136">Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-136">This triggers hybrid sort for messages : the first 3 messages are the most relevant.</span></span> <span data-ttu-id="7cdf8-137">Essa propriedade só é aplicável a entityType= `message` .</span><span class="sxs-lookup"><span data-stu-id="7cdf8-137">This property is only applicable to entityType=`message`.</span></span> <span data-ttu-id="7cdf8-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-138">Optional.</span></span>|
|<span data-ttu-id="7cdf8-139">entityTypes</span><span class="sxs-lookup"><span data-stu-id="7cdf8-139">entityTypes</span></span>|<span data-ttu-id="7cdf8-140">Coleção entityType</span><span class="sxs-lookup"><span data-stu-id="7cdf8-140">entityType collection</span></span>| <span data-ttu-id="7cdf8-141">Um ou mais tipos de recursos esperados na resposta.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-141">One or more types of resources expected in the response.</span></span> <span data-ttu-id="7cdf8-142">Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-142">Possible values are: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`.</span></span> <span data-ttu-id="7cdf8-143">Veja [as limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-143">See [known limitations](search-api-overview.md#known-limitations) for those combinations of two or more entity types that are supported in the same search request.</span></span> <span data-ttu-id="7cdf8-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-144">Required.</span></span>|
|<span data-ttu-id="7cdf8-145">campos</span><span class="sxs-lookup"><span data-stu-id="7cdf8-145">fields</span></span>|<span data-ttu-id="7cdf8-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cdf8-146">String collection</span></span> |<span data-ttu-id="7cdf8-147">Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e oneDrive, ou campos personalizados em **externalItem** do conteúdo ingerido pelos conectores do Graph.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-147">Contains the fields to be returned for each resource object specified in **entityTypes**, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in **externalItem** from content ingested by Graph connectors.</span></span> <span data-ttu-id="7cdf8-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-148">Optional.</span></span>|
|<span data-ttu-id="7cdf8-149">from</span><span class="sxs-lookup"><span data-stu-id="7cdf8-149">from</span></span>|<span data-ttu-id="7cdf8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7cdf8-150">Int32</span></span>|<span data-ttu-id="7cdf8-151">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-151">Specifies the offset for the search results.</span></span> <span data-ttu-id="7cdf8-152">Deslocamento 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-152">Offset 0 returns the very first result.</span></span> <span data-ttu-id="7cdf8-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-153">Optional.</span></span>|
|<span data-ttu-id="7cdf8-154">consulta</span><span class="sxs-lookup"><span data-stu-id="7cdf8-154">query</span></span>|[<span data-ttu-id="7cdf8-155">searchQuery</span><span class="sxs-lookup"><span data-stu-id="7cdf8-155">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="7cdf8-156">Contém os termos de consulta.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-156">Contains the query terms.</span></span> <span data-ttu-id="7cdf8-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-157">Required.</span></span>|
|<span data-ttu-id="7cdf8-158">size</span><span class="sxs-lookup"><span data-stu-id="7cdf8-158">size</span></span>|<span data-ttu-id="7cdf8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="7cdf8-159">Int32</span></span>|<span data-ttu-id="7cdf8-160">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-160">The size of the page to be retrieved.</span></span> <span data-ttu-id="7cdf8-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-161">Optional.</span></span>|
|<span data-ttu-id="7cdf8-162">sortProperties</span><span class="sxs-lookup"><span data-stu-id="7cdf8-162">sortProperties</span></span>|<span data-ttu-id="7cdf8-163">[coleção sortProperty](sortProperty.md)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-163">[sortProperty](sortProperty.md) collection</span></span>|<span data-ttu-id="7cdf8-164">Contém a coleção ordenada de campos e direção para classificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-164">Contains the ordered collection of fields and direction to sort results.</span></span> <span data-ttu-id="7cdf8-165">Pode haver no máximo cinco propriedades de classificação na coleção.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-165">There can be at most 5 sort properties in the collection.</span></span> <span data-ttu-id="7cdf8-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-166">Optional.</span></span>|
|<span data-ttu-id="7cdf8-167">stored_fields (preterido)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-167">stored_fields (deprecated)</span></span>|<span data-ttu-id="7cdf8-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cdf8-168">String collection</span></span> |<span data-ttu-id="7cdf8-169">Isso agora é substituído pela propriedade **fields.**</span><span class="sxs-lookup"><span data-stu-id="7cdf8-169">This is now replaced by the **fields** property.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7cdf8-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cdf8-170">JSON representation</span></span>

<span data-ttu-id="7cdf8-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-171">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7cdf8-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="7cdf8-172">See also</span></span>
- <span data-ttu-id="7cdf8-173">Pesquisar [mensagens de email](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-173">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="7cdf8-174">Pesquisar [eventos de calendário](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-174">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="7cdf8-175">Pesquisar conteúdo no SharePoint e no OneDrive[(arquivos, listas e sites)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-175">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="7cdf8-176">Pesquisar [dados de tipos personalizados importados usando conectores)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-176">Search [custom types imported using connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="7cdf8-177">[Classificar resultados](/graph/search-concept-sort) de pesquisa</span><span class="sxs-lookup"><span data-stu-id="7cdf8-177">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="7cdf8-178">Usar [agregação para refinar](/graph/search-concept-aggregations) os resultados da pesquisa</span><span class="sxs-lookup"><span data-stu-id="7cdf8-178">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


