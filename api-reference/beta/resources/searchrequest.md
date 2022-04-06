---
title: Tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta. Ele contém o tipo de entidades esperada na resposta, as fontes subjacentes, os parâmetros de paging, a solicitação de campos e a consulta de pesquisa real.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b8c91ce200e052850b0cbfefb7736e5bc3337e10
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589426"
---
# <a name="searchrequest-resource-type"></a>Tipo de recurso searchRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de pajamento, as opções de classificação, as agregaçãos e campos solicitados e a consulta de pesquisa real. Consulte [exemplos de](#see-also) solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas na](search-api-overview.md#known-limitations) pesquisa de combinações específicas de tipos de entidade e classificação ou agregação de resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição             
|:-------------|:------------|:------------
|aggregations|[Coleção aggregationOption](aggregationOption.md)|Especifica as agregação (também conhecidas como refinadores) a serem retornadas juntamente com os resultados da pesquisa. Opcional.|
|aggregationFilters|Coleção String|Contém um ou mais filtros para obter resultados de pesquisa agregados e filtrados para um valor específico de um campo. Opcional.<br>Crie esse filtro com base em uma pesquisa anterior que agrega pelo mesmo campo. Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}:\\"{aggregationFilterToken}\\".** <br>Se vários valores para o mesmo campo precisarem ser fornecidos, use as cadeias de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**. <br>Por exemplo, pesquisar e agregar itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de `docx` arquivo na resposta. Você pode convenientemente usar a `docx` **agregaçãoFilterToken** retornada para este **searchBucket** em uma consulta de pesquisa subsequente e o filtro corresponde aos itens de unidade do tipo de arquivo. [O Exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [e o exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.|
|contentSources|Coleção String|Contém a conexão a ser direcionada. <br>Respeita o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionId definida na Administração de Conectores. <br> Observação: contentSource só é aplicável quando entityType=`externalItem`. Opcional.|
|enableTopResults|Booliano|Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes. Essa propriedade só é aplicável a entityType=`message`. Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `person`, `externalItem`. Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção String |Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e OneDrive, ou campos personalizados em **externalItem** do conteúdo que os conectores do Microsoft Graph trazem. <br>A propriedade fields pode estar usando os [rótulos semânticos](/microsoftsearch/configure-connector#step-5-assign-property-labels) aplicados às propriedades. Por exemplo, se uma propriedade for rotulada como título, você poderá recuperá-la usando a seguinte sintaxe : label_title.<br>Opcional.|
|from|Int32|Especifica o deslocamento para os resultados da pesquisa. Deslocamento 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos de consulta. Obrigatório.|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|Fornece opções de alteração de consulta formatadas como um blob JSON que contém dois sinalizadores opcionais relacionados à correção ortográfica. Opcional. |
|resultTemplateOptions|[coleção resultTemplateOption](resultTemplateOption.md)|Fornece as opções de modelos de resultados de pesquisa para resultados de pesquisa de conectores de renderização.|
|size|Int32|O tamanho da página a ser recuperada. Opcional.|
|sortProperties|[Coleção sortProperty](sortProperty.md)|Contém a coleção ordenada de campos e direção para classificar resultados. Pode haver no máximo 5 propriedades de classificação na coleção. Opcional.|
|trimDuplicates|Booliano|Indica se os arquivos de SharePoint duplicados dos resultados da pesquisa. O valor padrão é `false`. Opcional.|
|stored_fields (preterido)|Coleção String |Isso agora é substituído pela **propriedade fields** . |

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
  "aggregationFilters": ["String"],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "contentSources": ["String"],
  "enableTopResults": true,
  "entityTypes": ["String"],
  "fields": ["String"],
  "from": 1024,
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "queryAlterationOptions": {"@odata.type": "microsoft.graph.searchAlterationOptions"},
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}],
  "size": 1024,
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "trimDuplicates": false
}
```

## <a name="see-also"></a>Confira também
- [Usar modelos de consulta](/graph/search-concept-query-template)
- [Pesquisar mensagens de email](/graph/search-concept-messages)
- [Pesquisar eventos do calendário](/graph/search-concept-events)
- [Pesquisar pessoa](/graph/search-concept-person)
- [Pesquisar conteúdo em SharePoint e OneDrive](/graph/search-concept-files) (arquivos, listas e sites)
- [Pesquisar tipos personalizados importados usando conectores](/graph/search-concept-custom-types)
- [Classificar resultados de pesquisa](/graph/search-concept-sort)
- [Cortar resultados de pesquisa duplicados](/graph/search-concept-trim-duplicate) 
- [Usar agregação para](/graph/search-concept-aggregation) refinar resultados de pesquisa
- [Usar layout de exibição](/graph/search-concept-display-layout)
- [Habilitar correções ort](/graph/search-concept-speller) spell nos resultados da pesquisa


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
