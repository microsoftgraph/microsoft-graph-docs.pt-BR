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
# <a name="searchrequest-resource-type"></a>tipo de recurso searchRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, as opções de classificação, as agregações e os campos solicitados e a consulta de pesquisa real. Confira [exemplos](#see-also) de solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas](search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|:------------|
|aggregations|coleção [aggregationOption](aggregationOption.md)|Especifica agregações (também conhecidas como refinadores) a serem retornadas junto com os resultados da pesquisa. Opcional.|
|aggregationFilters|Conjunto de cadeias de caracteres|Contém um ou mais filtros para obter os resultados da pesquisa agregados e filtrados para um valor específico de um campo. Opcional.<br>Crie este filtro com base em uma pesquisa anterior que seja agregada pelo mesmo campo. Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres na propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**. <br>Por exemplo, a pesquisa e agregação de itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de arquivo `docx` na resposta. Você pode usar convenientemente o **aggregationFilterToken** retornado para este **searchBucket** em uma consulta de pesquisa e filtro de correspondência subsequentes correspondem a itens de unidade do `docx` tipo de arquivo. O [exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) e o [exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.|
|contentSources|Conjunto de cadeias de caracteres|Contém a conexão a ser direcionada. <br>Respeita o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores. <br> Observação: contentSource só é aplicável quando entityType = `externalItem` . Opcional.|
|enableTopResults|Booliano|Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes. Esta propriedade só é aplicável a entityType = `message` . Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para as combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Conjunto de cadeias de caracteres |Contém os campos a serem retornados para cada objeto de recurso especificado em **EntityTypes**, permitindo a personalização dos campos retornados por padrão, caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e do onedrive, ou campos personalizados no **externalItem** a partir de conteúdo ingerido por conectores do Graph. Opcional.|
|from|Int32|Especifica o deslocamento dos resultados da pesquisa. Offset 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos da consulta. Obrigatório.|
|size|Int32|O tamanho da página a ser recuperada. Opcional.|
|sortproperties|coleção [SortProperty](sortProperty.md)|Contém a coleção ordenada de campos e direção para classificar os resultados. Pode haver no máximo 5 Propriedades de classificação na coleção. Opcional.|
|stored_fields (preterido)|Conjunto de cadeias de caracteres |Agora, ela é substituída pela propriedade **Fields** . |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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

## <a name="see-also"></a>Confira também
- [Mensagens de email](/graph/search-concept-messages) de pesquisa
- [Eventos de calendário](/graph/search-concept-events) de pesquisa
- Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))
- Dados [de tipos personalizados de pesquisa (conectores do gráfico)](/graph/search-concept-custom-types)
- [Classificar](/graph/search-concept-sort) resultados de pesquisa
- Usar [agregações](/graph/search-concept-aggregations) para refinar os resultados da pesquisa


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


