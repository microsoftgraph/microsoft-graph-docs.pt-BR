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
# <a name="searchrequest-resource-type"></a>Tipo de recurso searchRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paging, as opções de classificação, as agregação e os campos solicitados e a consulta de pesquisa real. Veja [exemplos de](#see-also) solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas em](search-api-overview.md#known-limitations) pesquisar combinações específicas de tipos de entidade e classificar ou agregar resultados de pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|:------------|
|aggregations|[Coleção aggregationOption](aggregationOption.md)|Especifica as agregação (também conhecidas como refinadores) a serem retornadas junto com os resultados da pesquisa. Opcional.|
|aggregationFilters|Coleção de cadeias de caracteres|Contém um ou mais filtros para obter resultados de pesquisa agregados e filtrados para um valor específico de um campo. Opcional.<br>Crie esse filtro com base em uma pesquisa anterior que seja agregada pelo mesmo campo. Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **\\ "{field}: "{aggregationFilterToken} \\ ""**. <br>Se vários valores para o mesmo campo precisam ser fornecidos, use as cadeias de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **\\ "{field}:or( "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**. <br>Por exemplo, pesquisar e agregar itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de `docx` arquivo na resposta. Você pode usar convenientemente o **aggregationFilterToken** retornado para esse **searchBucket** em uma consulta de pesquisa subsequente e o filtro corresponde aos itens de unidade do tipo `docx` de arquivo. [O Exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) e [o exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.|
|contentSources|Coleção de cadeias de caracteres|Contém a conexão a ser direcionada. <br>Respeita o seguinte formato: `/external/connections/connectionid` onde `connectionid` ConnectionId é definido na Administração de Conectores. <br> Observação: contentSource só é aplicável quando entityType= `externalItem` . Opcional.|
|enableTopResults|Booliano|Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes. Essa propriedade só é aplicável a entityType= `message` . Opcional.|
|entityTypes|Coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Veja [as limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção de cadeias de caracteres |Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e oneDrive, ou campos personalizados em **externalItem** do conteúdo ingerido pelos conectores do Graph. Opcional.|
|from|Int32|Especifica o deslocamento dos resultados da pesquisa. Deslocamento 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos de consulta. Obrigatório.|
|size|Int32|O tamanho da página a ser recuperada. Opcional.|
|sortProperties|[coleção sortProperty](sortProperty.md)|Contém a coleção ordenada de campos e direção para classificar os resultados. Pode haver no máximo cinco propriedades de classificação na coleção. Opcional.|
|stored_fields (preterido)|Coleção de cadeias de caracteres |Isso agora é substituído pela propriedade **fields.** |


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
- Pesquisar [mensagens de email](/graph/search-concept-messages)
- Pesquisar [eventos de calendário](/graph/search-concept-events)
- Pesquisar conteúdo no SharePoint e no OneDrive[(arquivos, listas e sites)](/graph/search-concept-files)
- Pesquisar [dados de tipos personalizados importados usando conectores)](/graph/search-concept-custom-types)
- [Classificar resultados](/graph/search-concept-sort) de pesquisa
- Usar [agregação para refinar](/graph/search-concept-aggregations) os resultados da pesquisa


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


