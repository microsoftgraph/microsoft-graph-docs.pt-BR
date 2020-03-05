---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fe3117eae0e514bea979281220da12820574cb4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520896"
---
# <a name="searchrequest-resource-type"></a>tipo de recurso searchRequest

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|stored_fields|String collection |Contém os campos a serem retornados para earch _so objeto urces. Observação isso só é aplicável quando entityType =`externalItem` é especificado na resposta.|
|contentSources|String collection|Contém a conexão a ser direcionada. <br>Respeite o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores <br> Observação contentSource só é aplicável quando entityType =`externalItem`. |
|enableTopResults|Boolean|Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes<br> Isso só se aplica a entityType =`message`.|
|entityTypes|coleção `entityType`| Os valores possíveis são: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.|
|from|Int32|Especifica o deslocamento dos resultados da pesquisa. Offset 0 retorna o primeiro resultado.|
|consulta|[searchQuery](searchquery.md)|Contém os termos da consulta.|
|size|Int32|O tamanho da página a ser recuperada.|

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
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
