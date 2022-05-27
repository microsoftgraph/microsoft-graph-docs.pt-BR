---
title: Tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta. Ele contém o tipo de entidades esperado na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0f981aedcea282e2956859412d4d9c7ad8730323
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694402"
---
# <a name="searchrequest-resource-type"></a>Tipo de recurso searchRequest

Namespace: microsoft.graph

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, as opções de classificação, as agregações e os campos solicitados e a consulta de pesquisa real. Veja [exemplos de](#see-also) solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas](search-api-overview.md#known-limitations) na pesquisa de combinações específicas de tipos de entidade e na classificação ou na agregação de resultados da pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição| 
|:-------------|:------------|:------------|
|aggregationFilters|Coleção de cadeias de caracteres|Contém um ou mais filtros para obter resultados de pesquisa agregados e filtrados para um valor específico de um campo. Opcional.<br>Crie esse filtro com base em uma pesquisa anterior que agrega pelo mesmo campo. Na resposta da pesquisa anterior, identifique o [searchBucket](searchBucket.md) que filtra os resultados para o valor específico do campo, use a cadeia de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}:\\"{aggregationFilterToken}\\"**. <br>Se for necessário fornecer vários valores para o mesmo campo, use as cadeias de caracteres em sua propriedade **aggregationFilterToken** e crie uma cadeia de caracteres de filtro de agregação no formato **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**. <br>Por exemplo, pesquisar e agregar itens de unidade por tipo de arquivo retorna um **searchBucket** para o `docx` tipo de arquivo na resposta. Você pode usar convenientemente **a agregaçãoFilterToken** retornada para este **searchBucket** em uma consulta de pesquisa subsequente e o filtro corresponde aos `docx` itens de unidade do tipo de arquivo. [O exemplo 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [e o exemplo 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) mostram as solicitações e respostas reais.|
|aggregations|[coleção aggregationOption](aggregationOption.md)|Especifica agregações (também conhecidas como refinadores) a serem retornadas junto com os resultados da pesquisa. Opcional.|
|contentSources|Coleção de cadeias de caracteres|Contém a conexão a ser direcionada.|
|enableTopResults|Booliano|Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes. Essa propriedade só é aplicável a entityType=`message`. Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Veja [as limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção de cadeias de caracteres |Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão; caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e OneDrive, ou campos personalizados em **externalItem** do conteúdo que os conectores do Microsoft Graph trazem. A **propriedade fields** pode usar os [rótulos semânticos](/microsoftsearch/configure-connector#step-6-assign-property-labels) aplicados às propriedades. Por exemplo, se uma propriedade for rotulada como título, você poderá recuperá-la usando a seguinte sintaxe: `label_title`. Opcional.|
|from|Int32|Especifica o deslocamento para os resultados da pesquisa. O deslocamento 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos de consulta. Obrigatório.|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|Opções de alteração de consulta formatadas em um blob JSON que contém dois sinalizadores opcionais relacionados à correção ortográfica. Opcional. |
|resultTemplateOptions|[coleção resultTemplateOption](resulttemplateoption.md)|Fornece as opções de modelo de resultado de pesquisa para renderizar os resultados da pesquisa de conectores.|
|size|Int32|O tamanho da página a ser recuperada. O valor máximo é 1000. Opcional.|
|sortProperties|[coleção sortProperty](sortProperty.md)|Contém a coleção ordenada de campos e a direção para classificar os resultados. Pode haver no máximo 5 propriedades de classificação na coleção. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "aggregationFilters": ["String"],
  "aggregations": {"@odata.type": "microsoft.graph.aggregationOption"},
  "enableTopResults": "Boolean",
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "fields": ["String"],
  "from": "Int32",
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "queryAlterationOptions": {"@odata.type": "microsoft.graph.searchAlterationOptions"},
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}],
  "size": "Int32"
}
```

## <a name="see-also"></a>Confira também
- Pesquisar [mensagens de email](/graph/search-concept-messages)
- Pesquisar [eventos de calendário](/graph/search-concept-events)
- Pesquisar conteúdo em SharePoint e OneDrive ([arquivos, listas e sites](/graph/search-concept-files))
- [Classificar resultados](/graph/search-concept-sort) da pesquisa
- Usar [agregações para refinar](/graph/search-concept-aggregations) os resultados da pesquisa
- Usar [layout de exibição](/graph/search-concept-display-layout.md)
- [Habilitar correções ortográficas](/graph/search-concept-speller) nos resultados da pesquisa


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


