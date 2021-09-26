---
title: Tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta. Ele contém o tipo de entidades esperada na resposta, as fontes subjacentes, os parâmetros de paging, a solicitação de campos e a consulta de pesquisa real.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3b45bbfb4b20f4422a24bb2d90c7279b06efd67c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763825"
---
# <a name="searchrequest-resource-type"></a>Tipo de recurso searchRequest

Namespace: microsoft.graph

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de pajamento, as opções de classificação, as agregaçãos e campos solicitados e a consulta de pesquisa real. Consulte [exemplos de](#see-also) solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas na](search-api-overview.md#known-limitations) pesquisa de combinações específicas de tipos de entidade e classificação ou agregação de resultados de pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição 
|:-------------|:------------|:------------
|aggregations|[Coleção aggregationOption](aggregationOption.md)|Especifica as agregação (também conhecidas como refinadores) a serem retornadas juntamente com os resultados da pesquisa. Opcional.|
|aggregationFilters|Coleção de cadeias de caracteres|Contém um ou mais filtros para obter resultados de pesquisa agregados e filtrados para um valor específico de um campo. Opcional.<br>Crie esse filtro com base em uma pesquisa anterior que agrega pelo mesmo campo. Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}: \\ "{aggregationFilterToken} \\ ""**. <br>Se vários valores para o mesmo campo precisarem ser fornecidos, use as cadeias de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**. <br>Por exemplo, pesquisar e agregar itens de unidade por tipo de arquivo retorna um **searchBucket** para o tipo de `docx` arquivo na resposta. Você pode convenientemente usar **a agregaçãoFilterToken** retornada para este **searchBucket** em uma consulta de pesquisa subsequente e o filtro corresponde aos itens de unidade do tipo `docx` de arquivo. [O Exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [e o exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.|
|contentSources|Coleção de cadeias de caracteres|Contém a conexão a ser direcionada.|
|enableTopResults|Boolean|Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes. Essa propriedade só é aplicável a entityType= `message` . Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção de cadeias de caracteres |Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e OneDrive. Opcional.|
|from|Int32|Especifica o deslocamento para os resultados da pesquisa. Deslocamento 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos de consulta. Obrigatório.|
|size|Int32|O tamanho da página a ser recuperada. Opcional.|
|sortProperties|[Coleção sortProperty](sortProperty.md)|Contém a coleção ordenada de campos e direção para classificar resultados. Pode haver no máximo 5 propriedades de classificação na coleção. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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

## <a name="see-also"></a>Confira também
- Pesquisar [mensagens de email](/graph/search-concept-messages)
- Eventos [de calendário de pesquisa](/graph/search-concept-events)
- Pesquisar conteúdo em SharePoint e OneDrive ([arquivos, listas e sites](/graph/search-concept-files))
- [Classificar resultados](/graph/search-concept-sort) da pesquisa
- Usar [agregação para](/graph/search-concept-aggregations) refinar resultados de pesquisa



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


