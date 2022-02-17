---
title: Tipo de recurso searchResponse
description: Descrição da pesquisaResponse
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b7d5668a86204e95e3f0f5e024ec985f98027ac9
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878649"
---
# <a name="searchresponse-resource-type"></a>Tipo de recurso searchResponse

Namespace: microsoft.graph

Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitsContainers|[coleção searchHitsContainer](searchhitscontainer.md)|Uma coleção de resultados de pesquisa.|
|resultTemplates|[coleção resultTemplate](resulttemplate.md)|Um dicionário de **resultTemplateIds** e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.|
|searchTerms|Coleção de cadeias de caracteres|Contém os termos de pesquisa enviados na consulta de pesquisa inicial.|
|queryAlterationResponse|[alterationResponse](alterationresponse.md)|Fornece informações relacionadas a correções ortográficas na resposta à alteração.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

