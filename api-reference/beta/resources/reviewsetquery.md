---
title: tipo de recurso reviewSetQuery
description: As consultas set de revisão são usadas para consultar e analisar dados armazenados em um revisor de descoberta eletrônica
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2030d2f3403af2967100cbbc7de2571b8493895d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510034"
---
# <a name="reviewsetquery-resource-type"></a>tipo de recurso reviewSetQuery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As consultas set de revisão são usadas para consultar e analisar os dados armazenados em um [revisor](reviewset.md)de descoberta eletrônica.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar](../api/reviewsetquery-list.md) | coleção [reviewSetQuery](reviewsetquery.md) | Listar as consultas de conjunto de revisão em um conjunto de revisão. |
| [Create](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Criar uma nova consulta de conjunto de revisão. |
| [Get](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Leia as propriedades e os relacionamentos de um objeto **reviewSetQuery** . |
| [Update](../api/reviewsetquery-update.md) | Nenhum | Atualizar uma consulta de conjunto de revisão. |
| [Delete](../api/reviewsetquery-delete.md) | None | Excluir consulta de conjunto de revisão. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| createdBy | [identitySet](https://docs.microsoft.com/graph/api/resources/identityset) | O usuário que criou a consulta. |
| createdDateTime |DateTimeOffset| A hora e a data em que a consulta foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| displayName | Cadeia de caracteres | O nome da consulta|
| id |String| O identificador exclusivo da consulta. Somente leitura.|
| lastModifiedBy | [identitySet](https://docs.microsoft.com/graph/api/resources/identityset) | O usuário que modificou a consulta pela última vez. |
| lastModifiedDateTime |DateTimeOffset | A data e a hora em que a consulta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| consulta | Cadeia de caracteres | A cadeia de caracteres de consulta na consulta KQL (linguagem de consulta de palavra-chave). Consulte para https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery obter mais detalhes.  Este campo é mapeado diretamente para a condição de palavras-chave.  Você pode refinar pesquisas usando campos listados no *nome de campo pesquisável* emparelhado com valores, por exemplo, *Subject: "Financials trimestrais" e date>= 06/01/2016 e date<= 07/01/2016* |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
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
