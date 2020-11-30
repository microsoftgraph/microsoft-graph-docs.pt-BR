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
# <a name="searchrequest-resource-type"></a>tipo de recurso searchRequest

Namespace: microsoft.graph

Uma solicitação de pesquisa formatada em um blob JSON. 

O blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, as opções de classificação, as agregações e os campos solicitados e a consulta de pesquisa real. Confira [exemplos](#see-also) de solicitações de pesquisa em vários recursos.

> [!NOTE]
> Esteja ciente das [limitações conhecidas](search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|:------------|
|contentSources|Coleção de cadeias de caracteres|Contém a conexão a ser direcionada.|
|enableTopResults|Boolean|Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes. Esta propriedade só é aplicável a entityType = `message` . Opcional.|
|entityTypes|coleção entityType| Um ou mais tipos de recursos esperados na resposta. Os valores possíveis são: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`. Consulte [limitações conhecidas](search-api-overview.md#known-limitations) para as combinações de dois ou mais tipos de entidade com suporte na mesma solicitação de pesquisa. Obrigatório.|
|campos|Coleção de cadeias de caracteres |Contém os campos a serem retornados para cada objeto de recurso especificado em **EntityTypes**, permitindo a personalização dos campos retornados por padrão, caso contrário, incluindo campos adicionais, como propriedades gerenciadas personalizadas do SharePoint e do onedrive. Opcional.|
|from|Int32|Especifica o deslocamento dos resultados da pesquisa. Offset 0 retorna o primeiro resultado. Opcional.|
|consulta|[searchQuery](searchquery.md)|Contém os termos da consulta. Obrigatório.|
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
- [Mensagens de email](/graph/search-concept-messages) de pesquisa
- [Eventos de calendário](/graph/search-concept-events) de pesquisa
- Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


