---
title: Tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade de consulta. Ele contém o tipo de entidades esperada na resposta, as fontes subjacentes, os parâmetros de paging, a solicitação de campos e a consulta de pesquisa real.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 41b8c643228a4080dec1d6e27a7c23467ec6263b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134476"
---
# <a name="searchrequest-resource-type"></a>Tipo de recurso searchRequest

Namespace: microsoft.graph

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de pajamento, as opções de classificação, as agregaçãos e campos solicitados e a consulta de pesquisa real. Consulte [exemplos de](#see-also) solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas na](search-api-overview.md#known-limitations) pesquisa de combinações específicas de tipos de entidade e classificação ou agregação de resultados de pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |             |
|:-------------|:------------|:------------|:------------|
|contentSources|Coleção String|Contém a conexão a ser direcionada.|
|enableTopResults|Booliano|Isso dispara a classificação híbrida para mensagens: as três primeiras mensagens são as mais relevantes. Essa propriedade só é aplicável a entityType= `message` . Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para essas combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção String |Contém os campos a serem retornados para cada objeto de recurso especificado em **entityTypes**, permitindo a personalização dos campos retornados por padrão caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e OneDrive. Opcional.|
|from|Int32|Especifica o deslocamento para os resultados da pesquisa. Deslocamento 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos de consulta. Obrigatório.|
|size|Int32|O tamanho da página a ser recuperada. Opcional.|

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



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


