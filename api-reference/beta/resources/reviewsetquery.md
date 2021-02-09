---
title: Tipo de recurso reviewSetQuery
description: As consultas de conjunto de revisão são usadas para consultar e excluir dados armazenados em um eDiscovery reviewSet
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f622f79c9103e704be93ffd97af37c1d188736f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153484"
---
# <a name="reviewsetquery-resource-type"></a>Tipo de recurso reviewSetQuery

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As consultas de conjunto de revisão são usadas para consultar e excluir dados armazenados em um eDiscovery [reviewSet](reviewset.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar consultas](../api/reviewsetquery-list.md) | [Coleção reviewSetQuery](reviewsetquery.md) | Listar as consultas do conjunto de revisão em um conjunto de revisão. |
| [Criar consultas](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Crie uma nova consulta de conjunto de revisão. |
| [Obter consultas](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Leia as propriedades e os relacionamentos de um **objeto reviewSetQuery.** |
| [Atualizar consultas](../api/reviewsetquery-update.md) | Nenhum(a) | Atualizar uma consulta de conjunto de revisão. |
| [Excluir consultas](../api/reviewsetquery-delete.md) | Nenhum(a) | Exclua a consulta do conjunto de revisão. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | O usuário que criou a consulta. |
| createdDateTime |DateTimeOffset| A hora e a data em que a consulta foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| displayName | String | O nome da consulta|
| id |String| O identificador exclusivo da consulta. Somente leitura.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | O usuário que modificou a consulta pela última vez. |
| lastModifiedDateTime |DateTimeOffset | A data e a hora em que a consulta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| consulta | String | A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language). Para obter detalhes, [consulte Os campos de metadados do documento na Descoberta Descoberta Avançada.](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)  Esse campo mapeia diretamente para a condição de palavras-chave.  Você pode refinar pesquisas usando campos listados no nome do campo *pesquisável* emparelhados com valores; por exemplo, *assunto:"Finanças Trimestrais" E Data>=01/06/2016 E Data<=01/07/2016* |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
