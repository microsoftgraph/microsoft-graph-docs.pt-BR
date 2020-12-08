---
title: tipo de recurso reviewSetQuery
description: As consultas set de revisão são usadas para consultar e analisar dados armazenados em um revisor de descoberta eletrônica
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 7ffea670daffb6c8ce53925096dbd4f2d4986477
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597255"
---
# <a name="reviewsetquery-resource-type"></a>tipo de recurso reviewSetQuery

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As consultas set de revisão são usadas para consultar e analisar os dados armazenados em um [revisor](reviewset.md)de descoberta eletrônica.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar consultas](../api/reviewsetquery-list.md) | coleção [reviewSetQuery](reviewsetquery.md) | Listar as consultas de conjunto de revisão em um conjunto de revisão. |
| [Criar consultas](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Criar uma nova consulta de conjunto de revisão. |
| [Obter consultas](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Leia as propriedades e os relacionamentos de um objeto **reviewSetQuery** . |
| [Atualizar consultas](../api/reviewsetquery-update.md) | Nenhum | Atualizar uma consulta de conjunto de revisão. |
| [Excluir consultas](../api/reviewsetquery-delete.md) | Nenhum | Excluir consulta de conjunto de revisão. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | O usuário que criou a consulta. |
| createdDateTime |DateTimeOffset| A hora e a data em que a consulta foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| displayName | String | O nome da consulta|
| id |String| O identificador exclusivo da consulta. Somente leitura.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | O usuário que modificou a consulta pela última vez. |
| lastModifiedDateTime |DateTimeOffset | A data e a hora em que a consulta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| consulta | String | A cadeia de caracteres de consulta na consulta KQL (linguagem de consulta de palavra-chave). Para obter detalhes, consulte [Document Metadata Fields in EDiscovery Advanced](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).  Este campo é mapeado diretamente para a condição de palavras-chave.  Você pode refinar pesquisas usando campos listados no *nome do campo pesquisável* emparelhado com valores; por exemplo, *Subject: "Finanças trimestrais" e date>= 06/01/2016 e date<= 07/01/2016* |

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
